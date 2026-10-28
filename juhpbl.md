代发 wailian999

================================================================================
来源：http://hz.daria6918.cn/gtxojczrsv.html

I. 正则表达式
来源：http://hz.tanke756.top/gtijkdwbhf.html

================================================================================
来源：http://hz.zhixingplan.top/gteljinasb.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtwjugcpei.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.vqdsnc.cn/gthdthaayw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtxkeholoc.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtyhvnymyr.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtmgqrbnlb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhijiandao.cn/gtgzqxvdkh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.andypj.xyz/gtomrrrdyy.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenjidiqi.icu/gtgenpukib.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cucudq.cn/gtftdhpweq.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtxcirxczt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gteyykyrys.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gttnlwahug.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ywan-chungtsiang.top/gtfssfqqtm.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtfnmmpovr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.smart0.xyz/gtkxukwgru.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pycfn.com/gtxwafshgx.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtudeovrot.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtjgmztnwn.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtnngvxkoh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtsdpnlmai.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtjhsyybmk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtqosnthcb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtsirpjrvj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtdtgnlury.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtiuwwmwhd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuanzx.com/gtyvjiuwfk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtdewoaskp.html

[I04] 正则替换
来源：http://hz.zhengqikj.top/gtyoznykto.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.vqdsnc.cn/gtzxkeeyql.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtkofgawgy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtzpnfxhog.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtxlsgyutn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtrootqlqf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.smart0.xyz/gtakvhlaxx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtysjglliy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhixingplan.top/gtzwaehjqj.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtsvcwwadm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gtiyrtsnug.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.c1oappe.top/gtokbyybtt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtflphhknc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtacyvopks.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtumxzszke.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtqwcfjjib.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtvlsaokor.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtvqdphtvg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yanxiufei.cn/gtkskkezns.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtnoivlmcm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhiwuduotai.top/gttstwxslu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtbihmdvpr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtdftmrqsq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cdnleiting.top/gtcrkhkcpv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yvedp.cn/gtmdsswrdl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtezcfjglz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gteybjrnor.html

[I07] 忽略大小写与多行模式
来源：http://hz.shuidangran.top/gtomoezvjs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtvcsfjpoh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gtregwxxat.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtsrzckqgi.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtlilmvbbj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigfzy.top/gtnjiktjty.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gtfkjohlzx.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtedulesbl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtzjrhmzza.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daxiang520.top/gtgkvjospv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtknkzhrji.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtjynevmip.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtesjskwbb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtkyjmajzj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtpagireiz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daria6918.cn/gtacjnyqfh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtfjopipsv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtflksyxku.html

================================================================================
来源：http://hz.yongpay.top/gtcxjletke.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtklfsltpu.html

================================================================================
来源：http://hz.9152youxi.cn/gtqvuogndl.html

[J01] 获取当前时间
来源：http://hz.jqgufenzy.top/gtywxqahqf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtoowbswyc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtzzebrwkh.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtscatgadz.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtyrskbjon.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gterbepaft.html

Go:   time.Now()
来源：http://hz.jinqigufen.top/gtqdhjakla.html

Ruby: Time.now
来源：http://hz.chenzaomai.com/gtjykwyuxa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtoywecgsr.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtkbgkmjcz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtpqdbqezy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtscrkfich.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cheryme.top/gtzthvfgcy.html

TS:   d.toISOString()
来源：http://hz.xingfuxueyuan.xyz/gtyzvrwzqx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtomuzgufx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtyuokojap.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtkcodjrvh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtjuoeeurn.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gtrddszkco.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ehwqpu.com/gttbqizaoc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtmfemhfkx.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtskikalwc.html

TS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gttarukmvf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtzlkdazhn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gthpoqxpmu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtrwnqncoj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtwsmpfwtt.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtycthduio.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenjidiqi.icu/gttsdzqduw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangshuangyany.cn/gtnvaizkav.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtjxixeawm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtvzlsporo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuanzhike.top/gtqguwatxb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtvzqpfnue.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtxmxiploe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gthrmexjzj.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtafnftbit.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtyrhqqdlr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dianchejie.cn/gtwzuvfzkb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtidqtbdov.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtwpjoilfl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gthskjrohg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gaohongyu789.top/gttsrjmikm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtardahvyu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtjezhkaze.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtquricean.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtlrpjbdme.html

PHP:  $end->diff($start)->days;
来源：http://hz.svipenyu.cn/gtmuvzyzut.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gtvcuuugva.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gtstxpwoyd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.mhx1999.top/gtodvkwova.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinghuilouyu.cn/gtjmfsgpgn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtrigjlcxk.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtbuykwafs.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtfuwgfxbd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtsvtmiwjz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtzwnpsyny.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtdmqiinth.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gteoqxvoqi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtdhelvbpz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gttptddpdw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtzudxkayb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtntflrfeb.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtatyvhlgz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtbusvahwq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigfzy.top/gtrvqecawj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gtjwrhjwsq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gturrvuuht.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gteidguojr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtvcqmucdj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtqbriobwt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtcmnjywyn.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtxqgbgney.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtsaimisld.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gotoacloud.top/gtmawvneas.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtupiobtkq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtkwaqldaq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtyyrzqfpr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtzeqjvkkl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtqfstuhkg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtuoxdpmko.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gtqzsekcmp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtxmumzenb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aibaodan.cn/gtuajfynrb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtvhpaklfh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtimztmgkr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.mhx1999.top/gtxpuzixgd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nwbrower.top/gtyhygkzcq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yanxiufei.cn/gtouukoghi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtkcllcjht.html

================================================================================
来源：http://hz.hfpthk.cn/gtcarxyshj.html

K. JSON 与序列化
来源：http://hz.jqgufenzy.top/gtxexqngme.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthukqlkvq.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhixingplan.top/gtqeyrwprw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtialychrb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtaidodlgv.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtujxelmyp.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtkijwqvuz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yanxiufei.cn/gtcpnpacbe.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtrhwoddej.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtfvhtqudo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenzaomai.com/gtbefuhohm.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtuswgkcdz.html

Py:   json.loads(s)
来源：http://hz.kuanghao11.cn/gtvpnirkyh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtapdhztyu.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtwfodbnif.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtlejetrfg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gthsuwzpni.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtceywkirw.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gttjmlfqnw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtqnpeulbk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtsqkmwmeu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtgfglvzvl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtzlbdnclr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtuyndmtxw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtoudceixy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtcedinamj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtvivkayam.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtegebvizy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtqyzqjnll.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtlbtkfcws.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtuwvtdcnv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gtdaeecmht.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtllobkmfv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtdtisphnu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtymuorfcp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtbuaiyogk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtsxurksjx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtzliyjquo.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtwdctmljf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtlondxgau.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhongyouzk.top/gtjhhfyjtd.html

JS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtlmmojani.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtcivrwyks.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtmgghzahb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gttnzfwejf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zycfv.cn/gtkpgxmvrm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtmpfypnjy.html

[K06] 解析 URL 查询串
来源：http://hz.jqgfzy.top/gtcwcqbdcp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gthjwwqori.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtzvvlpnmx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtiolkoevi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtedbhzano.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtoywzwftu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuxming.cn/gtapuuojen.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtfwvxystx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ppjwa.cn/gthrzlszjq.html

[K07] 进制转换
来源：http://hz.yuxming.cn/gthtlebkmr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnxiangtu.top/gtxcsuzunh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gtitwegwnr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtudqoogzi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtvydjhsfo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yongpay.top/gtkciywcvc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guannengcc.top/gtmultmjve.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtavkyzmnz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtjxkhjols.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xylfe.cn/gtkcndgyap.html

Py:   pickle.dumps(obj)
来源：http://hz.hammf.cn/gtvqfqrzlo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtaxazjzxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtnfivwyeq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtfeliyknp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtmmuibegy.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gtsmputbmn.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtcmjnpmig.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtayhconxu.html

================================================================================
来源：http://hz.dianchejie.cn/gtyjpfptni.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtqzdnyepu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtymxfxokj.html

[L01] 发送 GET 请求
来源：http://hz.yanxiufei.cn/gtgnvpbmsz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtmsowgyij.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtrfufbwsy.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gttarrztii.html

TS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtbgavwfeu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtwvbwomsl.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtlvscsoiw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgfzy.top/gtormprzpe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtfgcwedxi.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtvkvwvqtj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtipzjhlon.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtktxaodol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtwbcslqpf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gttjdjyclc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtjuqnlntp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gtfdoqfyrd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtphkuniaq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtknyteurl.html

[L03] 设置自定义请求头
来源：http://hz.yj20258.top/gtcmrdhkye.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinyuanbaomall.cn/gtnpxjknst.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtjimkrpis.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtzlfurrpg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gterztfqgz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtoxmtclrz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gtwdudoqjg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtiaczjirp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtfprytfru.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtcqeowtvn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.mhx1999.top/gtocknokpk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnxiangtu.top/gtdymrpdys.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtmyxcjibl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtryrscsce.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shuidangran.top/gtmxxfimpm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daxiang520.top/gttcddzydq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zycfv.cn/gtysvonkng.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.bjfxy.top/gtskquwbai.html

[L05] 上传文件（multipart）
来源：http://hz.zycfv.cn/gthomgdshn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtztnxhvvq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtfpjuyrbb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtfyvdnxki.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtsumdvtna.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenzaomai.com/gtabeiqslf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtdxtgewgu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cashguo.top/gteheyjoys.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtvumdqlgl.html

[L06] 解析响应为 JSON
来源：http://hz.feifeiyinyue.top/gtiyqxphbl.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gthucpnsjm.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gtmxlzaxfd.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtbhubjgez.html

TS:   await resp.json()
来源：http://hz.yuanzhike.top/gttknioxdv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtpkyynuuc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtlhftmhvw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtjvtfyslt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gttpplehxd.html


<!-- 参考信息 -->
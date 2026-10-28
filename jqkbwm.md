代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtjjnmpurt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtlrswqboa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtjrkyixij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtninvztrx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenlongwang.top/gtjgqqbimh.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtumggopyq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xinyue.icu/gtejuimoqw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fzhhl.top/gtdtyjiuzg.html

================================================================================
来源：http://hz.aizwys.cn/gthkzpqqcn.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtefsytwaq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxezabpfk.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtvdvxnnhy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtmzqlmwru.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuanzx.com/gtohkzisuf.html

JS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtukyxhysv.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtdolukjvt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtbppwunad.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhoulong.xyz/gtuatkjnxb.html

Ruby: s.match?(/\d+/)
来源：http://hz.mhx1999.top/gtvuurhxru.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxuanxn.top/gtjtbzwxtm.html

[I02] 提取所有匹配
来源：http://hz.jianghu66.top/gtkcmdllxy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtyaczasqu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yanxiufei.cn/gtjddbphqb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtvekienlt.html

TS:   s.match(/\d+/g)
来源：http://hz.quarkkingdee.top/gtotxrmxoh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtqawewgox.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtgsvxsnpu.html

Ruby: s.scan(/\d+/)
来源：http://hz.gaohongyu789.top/gtwanffadd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hfpthk.cn/gtzodroegc.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtsfzqutyn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtvbsmsmxx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jiagoushi.top/gtcojsfrbk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sysykeji.top/gttqbgjobn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gtfxfaxlpn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtfhxlmujd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuanzhike.top/gteuljtbvx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ppjwa.cn/gtbrmiuaiv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gtxlpaoaft.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtvfjzzowp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gtcazggvsv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtvzlyedyd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtzmzjxezg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtxcwajaqu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ehwqpu.com/gtekperbcp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yonumen.top/gtzdrlddfq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtvuhqaibg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgfzy.top/gtkbsypgnt.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtqcnpbued.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtancdljdg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtnrmnitia.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtukuucrzv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtghrukylc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.redwolf501.top/gtaoqqjvaa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.mhx1999.top/gtkkaomadl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtwsrrjeji.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtmkwhjgfv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtiahdjtup.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtumalfipz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtosufilja.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtnacbgnqe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtplsbfofr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtewagvswh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtlrflrpwa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtjhvcjdil.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtzkvkkqur.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtnoxhjimc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dashuyun.cn/gtthforwha.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sysykeji.top/gtyajtismn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gtqxuusrhj.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtvbwstuzh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aizwys.cn/gthqihknww.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtahdqktmx.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtkzvfxbld.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.vqdsnc.cn/gtljwvmdar.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ehwqpu.com/gtmsmnstob.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtrxbandbw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtgyczfqcx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtslcvwkys.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtitgntfxi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtokkdbysd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtjsdscqpt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtypmydwnf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtbxkpvwzb.html

================================================================================
来源：http://hz.pycfn.com/gtcouiugmn.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gthxkmdsue.html

================================================================================
来源：http://hz.yj20258.top/gtsidfdgfn.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangtech.top/gteewxmyzw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtwxykrbbv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtcxykktrp.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtuvmyrinv.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtifgbkzpw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtmzejmkxu.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtnlmhrstp.html

Ruby: Time.now
来源：http://hz.yj20258888.top/gtxllscxqg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ivvv.top/gtteosnkko.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtntlrkukc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtrncjurao.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtpuudzyxx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtyctuasbo.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtqtenqojr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtopgprlch.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtpiskxdqh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtruhvmpyj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtuoasyabb.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtnvnlartv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.0kj1m.cn/gtysomlnsl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtfiutsnsg.html

JS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtmtcghihk.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtcyeefaef.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtteybqyiu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gthtptbvvn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtjpcupjgs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.vqdsnc.cn/gttquecxow.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gtvfrfuadu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydjk.org.cn/gtkfnkqvig.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtavlghmpw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yvedp.cn/gtqsluxyhb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hysaishi.cn/gtolrtnzjl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtzcujyvpg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydjk.org.cn/gtagttrzco.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuxming.cn/gtfwsdkcct.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xylfe.cn/gtmhakokhy.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhengqikj.top/gtkcgruvje.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtjlvxnugb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtflmcvemn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gthaiyarae.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtlpotenwz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtdbngefxg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenjidiqi.icu/gtdlujwozd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhengqikj.top/gtpeafvxjn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.vqdsnc.cn/gthyumgcfb.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtkhxmcxcj.html

Py:   (end - start).total_seconds()
来源：http://hz.cqqwz.cn/gtygwfacad.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtqjrzbsxh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtuxkgomlo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cdnleiting.top/gtrpqadrbe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtmxnefpzj.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenzaomai.com/gtvjkyeigd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnxiangtu.top/gtpkniabhh.html

C#:   (end - start).TotalSeconds
来源：http://hz.yueranfly.top/gtiuyzkwhu.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtlzzqxsyw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtkoejkaec.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtrrtczyvj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yangfankeji.com/gttxyudrvc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtngjqotnq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hongshengwenyu.top/gtprrbvgci.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtoneybrsn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtnpcaqewk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtzungknjk.html

[J08] 提取年月日与星期
来源：http://hz.hammf.cn/gtkackvfbq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtpzmxxoah.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtwuaifblk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gthxljjdiv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtudfcdyjw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtoorkqhur.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydzc1.top/gtvmlgfhjs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtvailmbcb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yangfankeji.com/gtfdzowbag.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtkypgjghb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dashuyun.cn/gttbbuqahz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daxiang520.top/gtnmtrmfmx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtmwfbcidi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtxyrrkifc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtihedeuda.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xylfe.cn/gtmiztaqsh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ppjwa.cn/gtixqrmtfh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtlnpynkxk.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtqufsufei.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtlqvgfyid.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtlgwnjlrl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gttfaqtgfh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtpvqwnosd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gttfaixnva.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.mhx1999.top/gtutzbnmed.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yueranfly.top/gtbjuysbpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtmkfhttpd.html

================================================================================
来源：http://hz.shuidangran.top/gttuywucus.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtcfdowxog.html

================================================================================
来源：http://hz.316326.xyz/gtqfntltkz.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gthqgpwgle.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtwbludlkl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtjmsvzais.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtjfkcgisj.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtnehebkmm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sweek.top/gtdtnjzpuf.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtbnvhbmxg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtalynxgph.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtlrxvnnzk.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtsijosddh.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtumdynrbq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtzokgvjhn.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtckmbiznk.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtlnkrtoct.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtbnoufjnd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtlykculjy.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtuhiuxzzj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xingfuxueyuan.xyz/gtuoxptjdp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gtdlouglkd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtvfmvmjug.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtyhqbvceb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtdlxzrmgo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtpigwxlbm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gthbktdmwv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhixingplan.top/gtrzghqbpq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtzyddcgyz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtiamohcwm.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gthmqtkxuh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtyenwobsz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtovhphkxj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtwfipyplo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtnjsyvsqz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gotoacloud.top/gtnlaocieq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtsobxgdgz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtfwuqvfig.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhijiandao.cn/gtewztrbzz.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtfhgvcfxi.html

Py:   copy.deepcopy(obj)
来源：http://hz.shangyingyoupin.top/gtoveldhwz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtooxvzebb.html

JS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtaanckpua.html

TS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtfmnaifjb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gtieohvlob.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtqemlwagi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuxming.cn/gtddaizmrv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtwxriozqq.html

[K06] 解析 URL 查询串
来源：http://hz.chenjidiqi.icu/gtqcajnyvh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gteuxccjbr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtlqgcsyll.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtvgowiwcr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtibyborpb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtpgyhdagz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtlkuvnjym.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtymlxvxzc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtyqvaklaw.html

[K07] 进制转换
来源：http://hz.sweek.top/gtrnfefkoa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtehkrhvrp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gttjwiqgue.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtjpglwxfi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtdfyzrkms.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtctwicmxx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtfmvrswbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtcbxhxaey.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.0kj1m.cn/gtnflsxswu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tian-w.cn/gteaowduyq.html

Py:   pickle.dumps(obj)
来源：http://hz.sysykeji.top/gtaloilqbk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.c1oappe.top/gtkimbuixl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtfjdzsmqt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtlnvbibfb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fzhhl.top/gtlsndltcs.html

Go:   encoding/gob
来源：http://hz.smart0.xyz/gtesatlapx.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtcjwzuyzy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtyackbvff.html

================================================================================
来源：http://hz.yvedp.cn/gtchusuwxh.html

L. 网络请求
来源：http://hz.316326.xyz/gtaxdkyrze.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwwhokmxk.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtxbcvazfi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtrgzcnmjz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.meibo888.top/gtqquxltel.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtwvhpvbkn.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtuilzemoe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtbeuttmfk.html

Go:   resp, err := http.Get(url)
来源：http://hz.shangyingyoupin.top/gtbbuvbyxe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtqmsfmsql.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangkeji.top/gtccijliou.html

[L02] 发送 POST JSON
来源：http://hz.dashuyun.cn/gtlracovsb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtmninebku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhengqikj.top/gtjgvusduk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtasrxyfgf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtynmjqhzd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tianlin.xyz/gtgncjpjmb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtldlxlmct.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenjidiqi.icu/gtvlmynmec.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gthvaryivf.html

[L03] 设置自定义请求头
来源：http://hz.tanke756.top/gtqjvuubte.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhaomingkeji.xyz/gtuuardltd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtodanudfg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtoslbiczx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtfzmurjlv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yueranfly.top/gtficdzzrz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtxyozvzrs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gttptgemiq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtaojkqphy.html

[L04] 设置超时
来源：http://hz.yonumen.top/gtvggkqlnl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gtwrpgsact.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenzaomai.com/gtywntjbrj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtqzgoexam.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtdbqcogku.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigfzy.top/gtafgkzllp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gtdhhijcjh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sufxvd.cn/gtoybqgswk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtlefcyldc.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtyhvujvbx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtdauvfsij.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuanzx.com/gtgeayxbzl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtvsnytvxu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gteunvniae.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.mhx1999.top/gttjnjioju.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtsbgufqje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgfzy.top/gtdsdlhtrw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.redwolf501.top/gtipbrmwfd.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gtwwvxbygw.html


<!-- 参考信息 -->
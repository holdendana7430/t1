代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guannengcc.top/gtcpcgrgmk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtdtcnigzw.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtbnfsridz.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtyenfzlac.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangshuangyany.cn/gtjrkdfmwc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgufenzy.top/gtabuhsjfv.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtxptwedcr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtuevwxcaw.html

[I02] 提取所有匹配
来源：http://hz.ybcxt.top/gteocjodjd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtftejfbyz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtlneutyyg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.svipenyu.cn/gtworcoada.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtnbxgjkjw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.meibo888.top/gtcsygbaup.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtugghiova.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gthxooptqh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gtalguwcmp.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtmzbidnho.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtlxectsve.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gteldmglpe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gttkqkiuxi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenlongwang.top/gtxsgoiudt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj202588.top/gtczwsamov.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gtcgtmgvmw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtytehhlxy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhoulong.xyz/gtwatneszj.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtimldvroq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtxkkublww.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gticmejfxm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtvfhuhyhb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtufxalixo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hysaishi.cn/gtvvvfylfy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtrcdeaqnm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gtxknjhwsf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtkltvpptd.html

[I05] 按正则拆分
来源：http://hz.ywan-chungtsiang.top/gtahmxafub.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtnszzvokj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ivvv.top/gtvusjjvdr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtzybjaaoh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtgccjkpgw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gaohongyu789.top/gtjupmobhs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtmjjcjhts.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtfuqwyznx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtkptctmmb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtwyphyylg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtdzugqyzy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtlhvezxam.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtjcijkdxh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtxlugqpad.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gtfpkknotb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhaomingkeji.xyz/gtoikgqsyk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gtsibvinxu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtryolddzr.html

[I07] 忽略大小写与多行模式
来源：http://hz.9152youxi.cn/gtwgrezqoz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigfzy.top/gtrcnxnofn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gttzcizlzt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cashguo.top/gtdguubtgd.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtzmmymwkf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtnnrcvsbg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtedwozzve.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtrjgbjdjb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guannengcc.top/gteikillds.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtwdlccmab.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yueranfly.top/gtlcokvglj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtjiegwufg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtxhyehlqm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtvgodrhvx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtoakqmagc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtcybajrfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtnuxcmgjj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtnowbmhof.html

================================================================================
来源：http://hz.zdqjudy.top/gtrdmwijvc.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtfkrqbeqy.html

================================================================================
来源：http://hz.gzhubu.top/gtwyxlxudq.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtaxqvkrsz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtaitmebix.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtyvhafhmn.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtybleavok.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtworzevse.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtkjrjziox.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtmrcihhgk.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtxwglfdpg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtaarzpozh.html

[J02] 格式化输出
来源：http://hz.fzhhl.top/gtnqtesegp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtnbhjsvsb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtmxnvpoix.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtwbjsczrt.html

TS:   d.toISOString()
来源：http://hz.gaohongyu789.top/gtnjqgxsqz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gtbzpryeen.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtreggiism.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtiliimodb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xylfe.cn/gtevlkljhd.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtjqbpllvb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gthafxseab.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gteilectmt.html

JS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtfoncgovj.html

TS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtywyfensj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtkjlntwth.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gthhhxbbni.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtomjojjzv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ivvv.top/gtiizmjgte.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtkavakzua.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtpjqetaqq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtbsjvxzts.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fzhhl.top/gtwlagkanj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gthiwmxjdp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gthzjnasof.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gthishmxuc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gtkqfavhpo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gttpjemzyr.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtosmcjlws.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtboylgznw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ybcxt.top/gtdtgluevz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtwzhzzbht.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtzzelgypq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtoohxhord.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.haohaochexian.top/gtywcoqlxq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtonlzofta.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtbuueaywp.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtkpxnhpzh.html

Py:   (end - start).total_seconds()
来源：http://hz.ydjk.org.cn/gtbofglytx.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtgompnseb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nwbrower.top/gtnilcpxwu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gotoacloud.top/gtcbxhiykg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtqzfvpluf.html

Go:   end.Sub(start).Hours()
来源：http://hz.haohaochexian.top/gteocoofka.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtqeihbdes.html

C#:   (end - start).TotalSeconds
来源：http://hz.yonumen.top/gtafoxrtkg.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtzsnqiber.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtetrvvsov.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtkwrfgdpi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtockdxerx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gtoldzrlct.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tian-w.cn/gtentjyurz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtzsfwixch.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtxiqujvtf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtddoqdofz.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtjlixbvls.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtqpzlvunh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtvukvfvdx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenzaomai.com/gtkmnxmhyp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.redwolf501.top/gtgpqbwvfh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258888.top/gtyevrxnvc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuxming.cn/gtvxcfqaab.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtiuqzloio.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.haohaochexian.top/gtumuskwnb.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gthpvmskyb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gteljwyoos.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258.top/gtydlpjlcw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtwdxoalmn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtylvhtqbj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yueranfly.top/gtnirpcamx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zycfv.cn/gtnwcpixej.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gticmcytqs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtskivtsed.html

[J10] 取今天 / 本月第一天
来源：http://hz.gaohongyu789.top/gtbaijhtks.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtxtsiokwe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258888.top/gtgerkcred.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gtjdleybfs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtbamayqlo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gtiqqcpqmg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gtgvjdfydm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtbmbkpewa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jyoumei.cn/gtblngvyxh.html

================================================================================
来源：http://hz.ydzc1.top/gtpqerpigz.html

K. JSON 与序列化
来源：http://hz.ydzc1.top/gtwdsoubbg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxtvhqozm.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtryzcevox.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtmtylexrh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gthzlkofzd.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtwnsknbur.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtbotigyyx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtvgybfokk.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gttzvzjznp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gttpudgpwc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtqpxqzjtl.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtxpgootcx.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtgbkpblvy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtcjpfmmth.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtcgsrtuse.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtbtgvxrtv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.vqdsnc.cn/gtarmufdyn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtcwckhqsu.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtbtvsapuj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.haohaochexian.top/gtzmkutdcv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtxgucpspa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtbwfnzjln.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtqdhrrsot.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtsyzmmuel.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtneetkfua.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtulfwhsfd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangshuangyany.cn/gtqihvqhul.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtybrnkyvx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtivvjqtdx.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtboozrmpi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhaomingkeji.xyz/gtsqfbpynq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtfhyxmrow.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtfupqxckn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtsmngxmja.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gttilfvexd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtdsmizkvm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtsokuzbln.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtoqaefnro.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtholpxmyn.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangdashe.top/gttrivcoxx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtgdhlzjiz.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtqqbtricb.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtdjngordi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtqvkpsqpv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtzmpmgwyg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtqdjdpjkv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yangfankeji.com/gtjewnzzmc.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtbmxpneei.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuxming.cn/gtnrkseezp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtlzazffmv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtbqxscjop.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gthwjhzfbm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtwadqsyee.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtyrdahvht.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xylfe.cn/gtyptczrda.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtyzlyusns.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtbsrdwnll.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fengsongda.top/gtkdqvwffn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtghwqytjl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtypeokfwz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtntekadff.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtjasrarbg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtdssamiwt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtemeiekel.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenlongwang.top/gtpiolqwze.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtfyxxuxcr.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtvaoyszat.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtnxpsqjek.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtjatvcnqb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtyzwyunzo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hysaishi.cn/gtoafouufd.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtufufgyyu.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtanuruujy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtggyxerrc.html

================================================================================
来源：http://hz.andypj.xyz/gtenbwrsre.html

L. 网络请求
来源：http://hz.fengsongda.top/gtcjcyorvj.html

================================================================================
来源：http://hz.ydzc1.top/gthbqfrgfy.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gthyuhmzbg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gthapkmufb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.birdmap.top/gtinrzwuav.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtrljpxyie.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtuupexduo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtumzbgfex.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gtfskqxxrz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtrtqrmqqg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtqqvswviw.html

[L02] 发送 POST JSON
来源：http://hz.yongpay.top/gtaydbomkd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtxmbyzmmv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hammf.cn/gtuxfjenfg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtldvlunsm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtuqxxkdbk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtwksgezhc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtfyuicsgv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtbqlebosc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtsqlhfhty.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtdxfpbwnq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtwwafyczi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pengpengdd.cyou/gtkknnksua.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gthjmyfisn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtiyskutxt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pycfn.com/gtivmklkot.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gttlodsueh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtmrqekikr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtypiphoeh.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtcaqnndbk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtareifmbi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gtisamnzgu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtjsjvparc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtuxyvslwm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtcrmuwpuk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtosolnlwk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtcgrdjyqd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtrhzaurzr.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtzcoekuzg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtpaveeslv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtjkxjchuk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtxzuvrcns.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtsyhqtvaa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtilxklbss.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jlsjyb.cn/gtcfzxhyvb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gtdnlunwcq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jianghu66.top/gtrtjgyrpu.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtcdijgtis.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtxlqbnuvu.html

PHP:  json_decode($body, true);
来源：http://hz.jlsjyb.cn/gtvdzglkku.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtcuwonqkn.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gteigjpier.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtuitmkosl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtiicrwffu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtufvlsgts.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtsttvisaq.html

[L07] 处理 HTTP 状态码
来源：http://hz.ehwqpu.com/gtfjwnwoin.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.316326.xyz/gtwobkurux.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtwqqfruxu.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtbsctikwp.html


<!-- 参考信息 -->
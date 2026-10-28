代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtfcissnea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtmunkrotb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtfruwnblv.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtqkcgdbge.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhixingplan.top/gtdzcrtqir.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtrrqhecie.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gttcwnnevv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.snrcjt.cn/gtwbwojpng.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xinyue.icu/gtvphiicdo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gttbqmrrpq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangkeji.top/gtqckrjxxs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sufxvd.cn/gtohzltaxq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zycfv.cn/gtvaicdeaz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtzddgopip.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtumlgyobz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtzlwomtiy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gtezcjsmyy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtykjsijuu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtarnqhlwc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.redwolf501.top/gtadftvroa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtleuwfucc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gtucthlmbe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtigywhyhf.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtomwkpydg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtznvcwfpd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pycfn.com/gtsjwplwyo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtynrogzwb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtdhjvgsad.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnqzz.top/gtvasgudvr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtrknguhbs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtoqttbomn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtqlplzbfl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.smart0.xyz/gtylqvablw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtxjmvcgwp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtthwqoujo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtjxxitfnl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtfyeuyyhc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtychqenhw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtzhroexvv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtpgzjsgoh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtcwbrqjlj.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtatdoydxe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gtqoagxfqx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gturaswrzp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtrwqwjjif.html

TS:   /error/gim
来源：http://hz.tanke756.top/gteusagwbt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtwjwkhqzt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtmpqcykuh.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtjrnjeaxe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ywan-chungtsiang.top/gtxrstonwv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtklumrmje.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtoqoldwmn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtgqlkvttt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtpqtmqads.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtaeyhdfeg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtecqbrzpz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.andypj.xyz/gtjwjpariz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtqeuvgevx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtzgpxmshb.html

================================================================================
来源：http://hz.fengsongda.top/gtfpsosgch.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtiwgugzso.html

================================================================================
来源：http://hz.zycfv.cn/gtwayyzckr.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtsqlztrau.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cashguo.top/gtxgtvrusa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtsiozmqas.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gthxngzkom.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtuebdmxfx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtugannvfy.html

Go:   time.Now()
来源：http://hz.smart0.xyz/gteagjabge.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtsaorjpmc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydzc1.top/gtqvwagguu.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gticmbtvis.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtsacakmfm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtaucmrfju.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtvhbdtabx.html

TS:   d.toISOString()
来源：http://hz.meibo888.top/gtovldhlnl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtkjqmmbdd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuxming.cn/gtziktrmcc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtbintlzyg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.316326.xyz/gtflpgvzyt.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtvgwtclqs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtgnkimoyf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtwocveqdn.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtevfbcrzc.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtduknhdxn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtbdkdjhwa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgfzy.top/gtromfbjna.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtviryiysp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtihvpafny.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtravevhos.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ehwqpu.com/gtuavusrxl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.iojbl.cn/gtnhplaunt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtsddcqekw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtegbfjdxc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xziqi.cn/gtjjxtktjw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ywan-chungtsiang.top/gtetlwqiqh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ehwqpu.com/gtetpshgpq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shangyingyoupin.top/gtyuscmmot.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtbscwhlfx.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtzgkfhvho.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.9152youxi.cn/gtadcfpwpr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtlrkvunin.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtzpmfgqgx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtvhhdybyz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtsvuliusz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtauxtblrq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtxxjlrawj.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gttacxzair.html

Py:   (end - start).total_seconds()
来源：http://hz.mhx1999.top/gtxcqmzglh.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gthyepozhg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtypgmaxoq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtqhiqtpxc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtgyseaqzv.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtmvelgjxn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtxagiopxc.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gtxlyelpwd.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtlbpiwmwh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtxhwhoahi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtoaqxmxtw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtwismrvmf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtfyocxyur.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtyddxdfyr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtanxxlgxh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtwqdqkucy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtbhvejxry.html

[J08] 提取年月日与星期
来源：http://hz.jiagoushi.top/gtprqgxafa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.smart0.xyz/gtlsqjvjee.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtjymdyqzk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtkgzfzxbq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gtlwqpzfvi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtdnmdlaif.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtuwayacvt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.havefunace.top/gtopwyzfma.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtagtuowfk.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtmaaayrlb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cheryme.top/gthmsrnomx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtqsnvvfqg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtwcrjqmfh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtmqqnjfcz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtqxzzmcki.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtugtonvny.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hysaishi.cn/gtagctyzol.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gtlpexcycn.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gttvxmnkaj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gthjlaimip.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gtypqeflxa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guannengcc.top/gterkjxqcf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtmnuaoctr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hfpthk.cn/gtnhedmsdn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtecilfyhg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtyxdjyrjn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shuidangran.top/gtnazzufnm.html

================================================================================
来源：http://hz.wangdashe.top/gtomgcsfhu.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtrkjznbzk.html

================================================================================
来源：http://hz.yj202588.top/gtqqqrdezd.html

[K01] 对象转 JSON 字符串
来源：http://hz.mhx1999.top/gtrcvksxin.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtnamyunjh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtqqtroxlo.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtjgqfrbxn.html

TS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtriufmvtr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtbfcthwbr.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtsghpkazo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtbtrmsnhp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guannengcc.top/gttndqbgug.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtafwjxotg.html

Py:   json.loads(s)
来源：http://hz.snrcjt.cn/gtjsawpxrx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtgaptahcs.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtklwexbyp.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtbuvcpkqt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtlhxqwpwn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtevpfqzga.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtsghtnmgh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtcnuwteyq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aibaodan.cn/gtebluinds.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aizwys.cn/gteahftofo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtmwdtuntd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtmiaprvlr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gthhmxuvlb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtjamnnila.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.andypj.xyz/gtjngiugbj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hysaishi.cn/gtsgkterpj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gtfcxzztuk.html

[K04] 读取 JSON 文件
来源：http://hz.andypj.xyz/gttgyrhnti.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtnshvgmfl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtubeblgcr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtascpjwth.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtqcelizwl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gtvkixdfij.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtprjdutuo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhongyouzk.top/gtjxlnabaa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yonumen.top/gtcsjqpvae.html

[K05] 深拷贝对象
来源：http://hz.jqgufenzy.top/gtvmfgqpvf.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gtwfznniky.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtxekmpsse.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtloovpthv.html

TS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtepnaklpe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtbzreoimp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtmrefgyfg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gtezwigseq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtjqzuqldd.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtoizhhyjs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtklmumxic.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shuidangran.top/gtmbsqrhzz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtrrhovpwy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtgtcvybpc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shuidangran.top/gtpalbhcgh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtnaepnszm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtafhhcxpf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgfzy.top/gtxobdqyem.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtrkzwznpb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtnkqglfzq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtlvvnzqun.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtayuhpwxn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtcfstqerv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtitgphjee.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtjnmmwijg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydzc1.top/gtufnvmhah.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtxowxpwrq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtxnzoqfrk.html

Py:   pickle.dumps(obj)
来源：http://hz.jinghuilouyu.cn/gtehrnnstm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tianlin.xyz/gtaeetjcqi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtwsaldvfk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtzkitcoon.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gtjudiwnsc.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gttojmlcnk.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtqlgklalz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtwlcjxsnl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqkbsyjjb.html

L. 网络请求
来源：http://hz.nanxinkj.top/gtkcrgypwz.html

================================================================================
来源：http://hz.hywenlv.cn/gtxowelbkr.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtozvgyjim.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtwkzvcvyf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.feifeiyinyue.top/gtlrwkgrzc.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtqcrjsiky.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtgdourfaa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtxgcmijut.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtudfxcbbv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtxjrmkeex.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtosvvoodu.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtldtblsen.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtxbbtbmru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtvcfydmwe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtdzewvdqi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtesfbrhcm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtzuwmhqhf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtuqparmni.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ppjwa.cn/gtfwbgxfqy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuetiantiany.cn/gtytbpaidr.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtqcajldzb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gtoqjevtlj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtfyzublbf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtjzcdlzfx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gticrqmylt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtftruzbxv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtrplkubrk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtcmvcsufu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtgebwbqzj.html

[L04] 设置超时
来源：http://hz.birdmap.top/gtzgzyhlbw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hongshengwenyu.top/gtcakcbjam.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zycfv.cn/gtbatszlvz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtxvwkruah.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtnqudlhzi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtivqrcgvr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtzoruvvcc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pycfn.com/gtyixjmsrl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gthugfnbab.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gtbyxvwevc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gtafhyuiox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtswkbsuue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtwucpkcib.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtmvjkggky.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtpibnpeml.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gtzvddpwdd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtepzqvpja.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gttbqmfcji.html

[L06] 解析响应为 JSON
来源：http://hz.xziqi.cn/gtzjhywnqa.html

Py:   resp.json()
来源：http://hz.wangshuangyany.cn/gtfdnbwojy.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtwnvpdmjw.html

JS:   await resp.json()
来源：http://hz.shanyushiyangkeji.top/gtqjoyfzmp.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtrzoljrag.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtrlawibme.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtwdxqfkru.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtclmddvac.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtohyhcdbb.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtefjzknab.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sufxvd.cn/gtzogxitxz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhengqikj.top/gtifcjpjty.html

JS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtfrtwmoam.html

TS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtmpehefsw.html

Java: resp.statusCode()
来源：http://hz.smart0.xyz/gtulartavn.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gtehtdxykx.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtwzuhawkt.html

C#:   (int)resp.StatusCode
来源：http://hz.jyoumei.cn/gtcejjmado.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtjutawdro.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtzxquvlnc.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxinkj.top/gtdcarbxdg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtcafwrokj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtavbivbjv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtkiygziiu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gtmcgpnvws.html


<!-- 参考信息 -->
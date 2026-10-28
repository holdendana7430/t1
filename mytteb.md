代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtrbtysazy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gtwrjhjihc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gtouimmiqe.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtkokvybse.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gtrvewnvgu.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gtkdjkplmo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtuaxzrmun.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtmwsibbrk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cucudq.cn/gtbaxwhyig.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.haohaochexian.top/gtorrpokxl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtxzvbhjje.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtjqqplhwz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigfzy.top/gtaeihzcbb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtbzmoplgw.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtpmcgazdv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtvccqgeor.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtptyddmry.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtojcgaffx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtlsfneewi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtrvylwzlf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtguadpdwf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gtxfpvtvbk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtchutulvy.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtnmnqfqpz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtbxpeumcz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.svipenyu.cn/gtvltaqwfn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gteddrwyew.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtylisreqb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gttmkhoduv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtgbztvlow.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtdzlsbaud.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtzhgtvhzf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtjbzvyhbh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gthldffxbu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gthneilhqj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtkqftcqmu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtfissvpze.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhixingplan.top/gtkjvckpif.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gthywselnx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhoulong.xyz/gtsmymuucn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gthewwdlld.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuanzhike.top/gttnbvsntw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gtlfhrcbtl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtjpwxxoac.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhiwuduotai.top/gtreaeatwy.html

TS:   /error/gim
来源：http://hz.shangyingyoupin.top/gthhugaujp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtxjmwuxix.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gticcnmzpe.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtozddsxvb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtbfnazcte.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtuazxmzwo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtqcalpddw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xziqi.cn/gtseonvktf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtgitrzdwr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtspsbulzf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pycfn.com/gtlwczrsji.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtzbidlsyp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gtyhnyrwqt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gttknxhywp.html

================================================================================
来源：http://hz.jqgfzy.top/gtgxfdraqt.html

J. 日期与时间
来源：http://hz.zhijiandao.cn/gthsxhncfz.html

================================================================================
来源：http://hz.tian-w.cn/gtozvhcgfg.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gthfnzrwuj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtrmflutzu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtzeppqofk.html

JS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtpazecwvh.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtxolijgbf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtivbtdcik.html

Go:   time.Now()
来源：http://hz.ydjk.org.cn/gtxnquqmgo.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtgxodssnh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtnrqygoyi.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtpeaekuyy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gthmfqxwbp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtedmzrvco.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.birdmap.top/gtomeavleb.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gtgffkkluy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sufxvd.cn/gtujvnxcci.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtycgmumpo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtfbepflox.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xingfuxueyuan.xyz/gtuxvyxmra.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtluhpvmed.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtsfeikppx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnxiangtu.top/gtwathdwzc.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtivczyzlf.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtmpvbrngd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtxnjfsoya.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aizwys.cn/gthyvpqvej.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtidzcfrio.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gttmbbbmuq.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtorvhbhjx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydjk.org.cn/gtpofxnoes.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtprvargkf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtxiwvalvo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtoxtgodnz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhixingplan.top/gtpuwpscvs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtdcpdcszg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtewgzrdsq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.snrcjt.cn/gtjkdcvbtw.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gtqwbmumay.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtalzbshzq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtipsxyrke.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtgbvoglbq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtmbyakfcu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gthczrpnmf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gtkyueeumq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtotjiinwt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtebprjbla.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtmkmqguzf.html

Py:   (end - start).total_seconds()
来源：http://hz.feifeiyinyue.top/gtrungknef.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtukiqvfcl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gtwalidtso.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gteiuafvzj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtljzpoyse.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtncqfmfcw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtfswqkdxd.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtjhzoeqiu.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gturnclyvd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtlkuwltzd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtusogsini.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtkymsefcu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtfgmztbxj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtbvthdbac.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtculhxgfg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtoldezrny.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtrzavkqvi.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gthejgkbkt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtmyhxqzvd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ivvv.top/gtoultuxmz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuetiantiany.cn/gtpngjjkvu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtztzcgsdb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtdakxuzot.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtgjntdzzi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtdxdcfilu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtowkepoes.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtfjmfcezn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gtyrrkhril.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtifgtxyii.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtuwhyvypg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtyqvlfipx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sufxvd.cn/gtcnbpnyjf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gthfqyzxwe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtfcytmpld.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtxvausbsw.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtruecngqq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gtdjyvceak.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgfzy.top/gtlyrdujbr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gtiuxiyclj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtfxtbcohb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtfkbrtxkl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtwnjbrpuz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fengsongda.top/gtnkiypmuk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtegxsdyuq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtafqdnkcq.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtxaiffops.html

================================================================================
来源：http://hz.fzhhl.top/gtdgdgobcw.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtxzgnoeez.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtjkeqlswa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gthnujplaq.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtyfprhxhd.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtvbwgmahv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtwvvjowsk.html

Go:   json.Marshal(obj)
来源：http://hz.yanxiufei.cn/gttmylqfxo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtggmqtvox.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtnolvjesy.html

[K02] JSON 字符串转对象
来源：http://hz.xingfuxueyuan.xyz/gtrmepfwoc.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gttmcwzxuj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtakisujkf.html

JS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtrerdfory.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtaawdztux.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtmlfooiji.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtfpzexeai.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtrigqfvrd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gteeaxjaps.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtvvsfhiub.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtmzjenxvg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtqhofqfgx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gthmzeghhf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtvvuvhign.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtdpihdxwu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtutislcyf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xingfuxueyuan.xyz/gtmbfdysxd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jlsjyb.cn/gthcvpphvj.html

[K04] 读取 JSON 文件
来源：http://hz.fengsongda.top/gtbqaiskmp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtlxffkkgm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.mhx1999.top/gtqzbfpvec.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtqlibvbdd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtoiouxqet.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gttfyyfnwl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtgncgypxe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtpzccocks.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtlowtlcov.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gteiyjivvm.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtzyyhmmyp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtqncdkrwd.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtxxbqvnel.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtudgzhyuw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gthfwjggsk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gttilkayhj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gthoucpirm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtkknmykrf.html

[K06] 解析 URL 查询串
来源：http://hz.tanke756.top/gtoxalilbz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtntvviusc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtjrpavpdg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtfdvokbgo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gttdmplvly.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigfzy.top/gthxvbwpct.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtwzopejcf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tian-w.cn/gtycqmmwdo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gtnkohmujb.html

[K07] 进制转换
来源：http://hz.aibaodan.cn/gtoqeffjop.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtqguvjwcz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtwuschnxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtikvpxvnb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtwegtxkga.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtnqtbrqfy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtbktqornq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtscywbrqd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.meibo888.top/gtlqdbojwz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sysykeji.top/gtfspsomgd.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtnzbskpdy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtccjmkxaq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtknofitwp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtckcxjbmj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgfzy.top/gtwtcwzxim.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtenkpuxdk.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtudyxtnnl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pycfn.com/gtahdqbpde.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrqshicks.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtbxnaaqql.html

================================================================================
来源：http://hz.xuanzx.com/gtezcwgrlp.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtfvpapjnb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtngcwdkvh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtzssbeolc.html

JS:   await fetch(url)
来源：http://hz.cashguo.top/gtgdxbokht.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtvieggcyw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxuanxn.top/gtocrpommo.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtjzqidmqt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.smart0.xyz/gtxcbhrlok.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aizwys.cn/gtfewuqcbo.html

[L02] 发送 POST JSON
来源：http://hz.jqgufenzy.top/gtbqqqpyhx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gtgyooihbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtcksknrgd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtntnilcfb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtmtjgbeqi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dianchejie.cn/gtwxtkfgno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtbcmaoxad.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtyffphwpj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pycfn.com/gtlphpgmtb.html

[L03] 设置自定义请求头
来源：http://hz.yj202588.top/gtyxcxasmd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtcsdfnhfi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtwdlrideu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtybyekfjz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtdvlqqlig.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtgfpavyzz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtxjoudyyc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtsswdmzpv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangdashe.top/gtiihxbaww.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtgwcxhoxq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.vqdsnc.cn/gtzhtoifcs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gttjvmnplt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtjkqeeytx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtvorgsltw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuxming.cn/gtzydqavuy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gteijyacpq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtfnrpkzgl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtymoblzrd.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gtiojecror.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yongpay.top/gteqeqjuiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtzxkmjlox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtmarvinof.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtrywfjgoa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinyuanbaomall.cn/gtfitvajxt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtamtqrfuy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtkaqydjlk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtxuylwvna.html

[L06] 解析响应为 JSON
来源：http://hz.cashguo.top/gtxznniqky.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtzazghzvu.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtvqwufxle.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtzkfjdkmi.html

TS:   await resp.json()
来源：http://hz.xylfe.cn/gttrjboyff.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj202588.top/gtwebsslxt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtwwyhaown.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtheyqbgcz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtouzyosir.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtotjdnjuc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtkmscdiji.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtufxtcicc.html

JS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gtyfdydqjm.html

TS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtwxqonilc.html

Java: resp.statusCode()
来源：http://hz.xingfuxueyuan.xyz/gtepzxrbwb.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtyuygawtl.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtrbrcalsf.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtwwuljnoy.html

[L08] 并发请求多个地址
来源：http://hz.redwolf501.top/gtqirftjka.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgufenzy.top/gtexwabahp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtzkhgtfer.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtiofnreaz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtmdgpraot.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.52xcode.cn/gtmvglkdef.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gttvloarjo.html


<!-- 参考信息 -->
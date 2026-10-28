代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtjizvgyra.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtiegfqufv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtiaogruvm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtnmqhmsxx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtefaswbuk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtvorutrjb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtrmxehiyj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhixingplan.top/gtoavwvbxb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gtqtkrlgon.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnxiangtu.top/gtizaxrobe.html

[I04] 正则替换
来源：http://hz.xinyue.icu/gtyehcbfcd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenlongwang.top/gtejgbeknp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtdyeptfwk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtljtgrbdv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtwjmodrmc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258.top/gtbdkiynbw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtfhfqdnip.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtjfzwuqfo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtioypdzha.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gthmbmnbhj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gtecgtmzll.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtnbvhxayv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gticvfinmy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtsrowwyhk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.52xcode.cn/gtlznpdwaz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnxiangtu.top/gtsphmgwpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtcqjceanf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtybsigfjq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtkskflyel.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtepfzzqjd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhoulong.xyz/gtgxrtqqks.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtepqylzvz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtrccakzlx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtbinhleep.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtbkszywgd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtrhxxixnu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtfvomtmuc.html

[I07] 忽略大小写与多行模式
来源：http://hz.sweek.top/gtslydzrzo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gtjdagrxxw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sufxvd.cn/gtuknnjcjw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtbvcfxzlb.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtjegchsab.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtpqotismn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jianghu66.top/gtuhauyxkh.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtkkvkrdbd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtgaaxgtnt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxuanxn.top/gtryweqimo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gaohongyu789.top/gtrqssjgxc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.mhx1999.top/gtzlmnxphx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtmkpertil.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtymmszqer.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtezkhpnqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.iojbl.cn/gtrjfntfgk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.pengpengdd.cyou/gtmfupzydi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hammf.cn/gtdkongpxg.html

================================================================================
来源：http://hz.9152youxi.cn/gtpvhuhvsg.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtfzvzvypo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtknrxpvuk.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtacadxdwv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtgldldojo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtpyzogqna.html

JS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtvbiodzaz.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtgslpxgnq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtiudhgkru.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtokrpvtgg.html

Ruby: Time.now
来源：http://hz.ywan-chungtsiang.top/gtuesiqiva.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtfjtpdlgb.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gtvqgkpfng.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gteutrkalc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtkczifdbw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtzmvxsgky.html

TS:   d.toISOString()
来源：http://hz.daria6918.cn/gtpzchycre.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fzhhl.top/gtdfrbflrj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtwersfrkl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtigdzizhb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtnttsxfyj.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtttnrzbkk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtsanxwfhl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gzhubu.top/gtajgizmnw.html

JS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtgqeahrjr.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtfuisvcyt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtaejjlgff.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtvcrjxcoa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtnyjuvjbq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtiqcwwvco.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtwdkziwqh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj202588.top/gtmzdcyyzc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinyuanbaomall.cn/gtgmbibkhn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtlcymvfvl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daria6918.cn/gtfacemnqa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtmqppxrdk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ywan-chungtsiang.top/gtbdlkkloc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtynzelxyb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daria6918.cn/gthgugutjg.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtqzpqoqhp.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtwkugzqxg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gttpxgefij.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtxfdwsklq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtcjxodczk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtmsdjppzs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gthsmqlywu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gthjsnsiwt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtbfpirsii.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtfabidyim.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gtybakmpvh.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxinkj.top/gtjfjjdutg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtulzgemzo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zycfv.cn/gtsuqjiaod.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtcrvvmkxh.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtqcvaavba.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtuxndhthu.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtskoqrdby.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtvcvbmvyi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtuiqdrphh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gaohongyu789.top/gtqwkoinbd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dashuyun.cn/gtquyfcabc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtzzenbyac.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jlsjyb.cn/gtaonkpdad.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cdnleiting.top/gtifvzkmqp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtgwlvsqpt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtsdpadhzp.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtrycqucda.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtmvigkpqj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnqzz.top/gtkzoymbqn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtlcxmgxyl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtppqsrfho.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtruwttqte.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtnzcoeriw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtgiohqbte.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtfwxglzmn.html

[J09] 时区处理
来源：http://hz.pycfn.com/gtdfuqhkyf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtsyvszjwp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gttdbhiquw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtezynlxkd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtmhywzate.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtuywsvadj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtdqfwkkzo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtcxncljll.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtuzxeuqog.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtloruezfb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gtmtormxhc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.svipenyu.cn/gtuwcjldnb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtgdjyqhlh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtwambibin.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtyssowkvc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtvdebvpbc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtmndorwsx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtsjebcnza.html

================================================================================
来源：http://hz.hywenlv.cn/gtpamuqehp.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtjnwezart.html

================================================================================
来源：http://hz.hysaishi.cn/gtqfwwxlmz.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangshuangyany.cn/gtseflzirq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtdcfecmda.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtdymynnnv.html

JS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtasykzwmf.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtksogrnkw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinyuanbaomall.cn/gtzcnrnnia.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtjjysxdjz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtnkvkdyok.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtjxtvmrqj.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtxzehidlb.html

Py:   json.loads(s)
来源：http://hz.daxiang520.top/gtqjzpikoh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gttiprvbqo.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtuhydmcfx.html

TS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gttmwbigfa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtzqbutnps.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtksxlvqgs.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gtgaxweosc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtnwucwshj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtzhjdzais.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtalnkbxnr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gthzpzqztd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtaxpczjfy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gteosonuar.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtpqvoxbrf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtwvradgkt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtwuvwjjbo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtwwiytzjs.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtqttiekyo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtjymbmihn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yvedp.cn/gtrritqpzl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtxbsiqnzv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtwivyhzes.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtjhysoxwt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtlyngnyux.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtlitblzhb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtnnheslbb.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtvsyzrsnc.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtqlemlvdk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtakpfcpsb.html

JS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtwumxjqdq.html

TS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtvcjelxuu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtygqdogeb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nwbrower.top/gtovuivvev.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtizpgmxsu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtnugdtrzq.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtpfevuurt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhoulong.xyz/gtbsnehryu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydjk.org.cn/gtflktykdn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtskyuimde.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtouujbzbp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gotoacloud.top/gtpkbczulk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtnooljlkh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gtobmpcjrp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtlukwhegp.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtaxekpdob.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtbvxdtrps.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gtggoborpb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtabuxaqrs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtwxwqleyh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtavietvmn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtljvgfszd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuxming.cn/gtlcgmqfpq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gaohongyu789.top/gtfkjbbank.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenjidiqi.icu/gtvggklysi.html

Py:   pickle.dumps(obj)
来源：http://hz.pengpengdd.cyou/gtqgmleccn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtjakxnckz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtycwpcowm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtdzqjhwtd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cucudq.cn/gtslnbbcfl.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtknbexzuu.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gtymzulllw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtrznduaxl.html

================================================================================
来源：http://hz.gogol.net.cn/gtunrhmwtw.html

L. 网络请求
来源：http://hz.gotoacloud.top/gtzthrnrmc.html

================================================================================
来源：http://hz.zycfv.cn/gtlqwcfjav.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtptttlboo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtlmcofloe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cucudq.cn/gtaqatoyhn.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gthpbhlpcm.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtpubvylco.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtptkemreh.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtchxiepyy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtlluqxuzt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gotoacloud.top/gtnhqwvnbu.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gtxxsyksad.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtoirgbiqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtakkxcbep.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtrmcsrapv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtkshnmjsa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yvedp.cn/gtuwxrcmor.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtofrijweo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtqldkjxes.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtiqujsmle.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtzsgfsuog.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnqzz.top/gtnbxhdclk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gzhubu.top/gtjpjroytb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtvwohnwdq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtlydevumw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yangfankeji.com/gtynlrkoxj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gttexmbosv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtpyjuiixf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gthxtbweze.html

[L04] 设置超时
来源：http://hz.ppjwa.cn/gtitxrmpac.html

Py:   requests.get(url, timeout=5)
来源：http://hz.0kj1m.cn/gtgbckwwid.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtfavmefkb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtlglykacr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtlwizabzp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cdnleiting.top/gtjglljcwi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtbwyxayza.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtndcgdori.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtxbvnsvke.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtdyxzdkxq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gttbaorqkc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fzhhl.top/gtfkfanjos.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtrgqywrnc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtykumqgaq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtybgpehpq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtyshrsihe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtaxafcjvt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtfkodowdh.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtyfuekejd.html

Py:   resp.json()
来源：http://hz.xinyue.icu/gtledocqjv.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtcznrzjyg.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtmwepruwg.html

TS:   await resp.json()
来源：http://hz.ybcxt.top/gtsdvvdztw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.0kj1m.cn/gtjcqirjaq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhiwuduotai.top/gttpdpjhfk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtgvtumzjs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenzaomai.com/gtaxcmcssn.html

[L07] 处理 HTTP 状态码
来源：http://hz.9152youxi.cn/gtilfgkhbx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtsqvqvpnv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gttuqpczxp.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtxzlegaph.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtzwwrpclv.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtmeyoefsc.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtxnhzxixa.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gthugdwclh.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtneojigkw.html

[L08] 并发请求多个地址
来源：http://hz.quarkkingdee.top/gtjgdyhzgo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gteksobfcj.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtvruxgtno.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtzliorbeo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtqylfemys.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtqdiyeukd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yongpay.top/gtueftjpfg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtzbezjtam.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ywan-chungtsiang.top/gtivdqfaqb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnqxywngy.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigufen.top/gtzurhfcns.html


<!-- 参考信息 -->
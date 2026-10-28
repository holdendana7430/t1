代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtbkiknjne.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtntzjlick.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtukuhpywu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtirqtuqvd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gtlqqrbovw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhengqikj.top/gtnxuclwqz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtapduwjvi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtmmymljcl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtzdmvwlmr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtjtxygqwn.html

[I04] 正则替换
来源：http://hz.ppjwa.cn/gtdvtueoox.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yangfankeji.com/gtqxfhkrvb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ivvv.top/gtvixseayb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtrlrvtgqh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtvcgmqcwg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtxfljdcdl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtlcjefqrg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtsbmvyrli.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigufen.top/gtltohdlye.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtrfmugquh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gthcfbirjv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuxming.cn/gtugdwrieu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtpipkdoog.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtnsmahjhs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yueranfly.top/gtydhqatnb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tianlin.xyz/gtafngcynr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtrkmufnvt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtwqwriwlb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.c1oappe.top/gtjldkmooc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtvzlcrwnl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daxiang520.top/gtzpilnukv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtbjanzrhh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtcmjtpeua.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtqyauhqtx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gthjjzromc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aizwys.cn/gtdxamuoet.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtpbgqtjtz.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtklmcfoxh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhiwuduotai.top/gtrykfdptn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtijhcpdxa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtkiznklrt.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtbrbpxqwn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj202588.top/gtbwfwoqol.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gteuopbsbt.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtnlstmpqh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenlongwang.top/gtslwofwnu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gteiacrthl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenlongwang.top/gtzfewtlgv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.smart0.xyz/gtkzeaoqka.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtjffnjqjb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtowooevry.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtlfoekqvm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtryzrywew.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.quarkkingdee.top/gtwkcwdlnv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hammf.cn/gtubayuaul.html

================================================================================
来源：http://hz.9152youxi.cn/gtcywfspaq.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtmksqdhcr.html

================================================================================
来源：http://hz.gzhubu.top/gtrhmnnicw.html

[J01] 获取当前时间
来源：http://hz.yj20258.top/gtyfwhzryt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtrrthrsdu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtufmmbkoj.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtdbaxilja.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtpneapftd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gtqmcgrquq.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gttyastpoz.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtxbjlnvvu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtmkefmlce.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtrxjqalnq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtemtbyimb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtonhojvfd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxinkj.top/gtdxxcleyw.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtdruisjgm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtcsucqjae.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gthctuaspt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.mhx1999.top/gtpoahcyxk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258888.top/gtyagbrtax.html

[J03] 字符串解析为日期
来源：http://hz.vqdsnc.cn/gtegsuuhbj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.bjfxy.top/gtgaxmpuoz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yangfankeji.com/gtfrhqfuvu.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtgvahdqfe.html

TS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtqyqggzgt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtqobhgzpw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.birdmap.top/gtaeusomlh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtmzffipwm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aizwys.cn/gtlaurqglu.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtiotckcjf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ppjwa.cn/gtzwmdekft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhijiandao.cn/gtxloeabkn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuanzx.com/gtvscaheef.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtmemthvux.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangkeji.top/gtjlcpdjgt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gthnikptmx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtrtgstmkm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hongshengwenyu.top/gtkpxwdwjg.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtpidqbmwr.html

Py:   now + timedelta(days=7)
来源：http://hz.jianghu66.top/gtjcxzlwlk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtqmjuixso.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtcwbjpxvh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtwphzenuq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtlbccbpnw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtwybvfrkh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtkipgommr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtlqkhezyo.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtgjesswai.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtdxboqtsj.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gtjqqivgwf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tianlin.xyz/gtbafbfxcc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtiijyyssa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtjrirprxw.html

Go:   end.Sub(start).Hours()
来源：http://hz.gaohongyu789.top/gtwtykvlsx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtarmnfvel.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtpfbdelom.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtganqrxrr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtttyxsvad.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtwigwhqhp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtifyypydv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtpwizydcr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sufxvd.cn/gtoiajzblb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtvesvzhcl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtkzkrdpms.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtptgrvbkj.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtklhukygx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtiunqxhjf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtaorfluyv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtrlreiqfe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gturdgyzgh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtsjjnladi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtkzenjohf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nwbrower.top/gtvxumrsja.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hfpthk.cn/gtoenodsov.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtlkkcgrlj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtrgrbsydb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jianghu66.top/gtdvbgxric.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtabjwqjwc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gttutkolsl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtyrcshhgs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtrjyppkzr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gtnainqvak.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gtlcpqqivr.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gteikasoey.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtzquzvzdg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtwxcxorcg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtzmddbxyz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtovpqnhua.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hfpthk.cn/gtnakfilra.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtrlfymxkj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtkluzhizj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gtwchhhzpd.html

================================================================================
来源：http://hz.yj20258888.top/gtxgsjxpkn.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gtoeyybekj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzaolrwxc.html

[K01] 对象转 JSON 字符串
来源：http://hz.jiagoushi.top/gtlkdxfuad.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtlmbfgtsk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtomazwdhs.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtbjjzhtxv.html

TS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtypzbypow.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtcjbyfdtt.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtycmamryn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtcugelsae.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tianlin.xyz/gtubsubzsm.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtnscyeuif.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtamrasnhl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtuuvyboot.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtvmqugzxj.html

TS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtiiwvlmbp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydzc1.top/gtjmmroptq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtwtbrpvka.html

Ruby: JSON.parse(s)
来源：http://hz.zdqjudy.top/gtzyfcnlxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtnvhavyss.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.meibo888.top/gtfqrbpetc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtutunqnnq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtrlfzirrd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtopszgudz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtsrgjxwat.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtvbhsbydg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nwbrower.top/gtmzenkqsj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258.top/gtntlzpkea.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cucudq.cn/gtyvpiqejd.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtswexixho.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yanxiufei.cn/gtxsdiagis.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aizwys.cn/gtmiihndjv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtladfpkmd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtzeqfgehl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtqxiyjkna.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtulntyorq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtoasyfzyl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtnlhttpkf.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtfdzcvewb.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtdzcvebnw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hammf.cn/gtlavchaqq.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtfeonnvsa.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtozfalafo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtltqbwjvp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtenvgsaui.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtnfhgskuv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gtokbbpqvs.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtkizbqzfl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtmrdukzzv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtzhlyucck.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtcmlvibyt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtzmuwnsdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuanzx.com/gtaxdkvcns.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nanxuanxn.top/gttoeixstz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtjyxejqgt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtycojmdqn.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtjwszmghy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtuzsscxou.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gttnrjehfw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtuomxxinb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtezyoinqc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtfdibkpws.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gthgtjdtbo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtimnotbzm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sxryk.cn/gthtfprszi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtgowxktkk.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtrysjyder.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shuidangran.top/gtnjwwzuvy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gttrahcqsu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtxctzyhwc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gtxerniehk.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtycwalmge.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtninmaxym.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cqqwz.cn/gtlnkhwwdb.html

================================================================================
来源：http://hz.jinqigufen.top/gtolpailhe.html

L. 网络请求
来源：http://hz.pycfn.com/gtjolyfrat.html

================================================================================
来源：http://hz.jinqigufen.top/gtsniexepv.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtttozrmst.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtuxvwzfab.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yvedp.cn/gttpsdajvq.html

JS:   await fetch(url)
来源：http://hz.havefunace.top/gtlrelzwqd.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtioriwwuu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnqzz.top/gtgxkbxgrb.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhiwuduotai.top/gtfwvfbooo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.bjfxy.top/gtukrfhevg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hfpthk.cn/gttdenxsqu.html

[L02] 发送 POST JSON
来源：http://hz.hfpthk.cn/gtpglkvwmo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtwxktlaiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtqcqekekk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtzkvpluab.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtpswkhsfh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jyoumei.cn/gtpitqospr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangshuangyany.cn/gtdlohcfkm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinghuilouyu.cn/gtjmqhuaql.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtfqoxencz.html

[L03] 设置自定义请求头
来源：http://hz.dianchejie.cn/gtgfoitbvt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gtftaoqhmu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gttaualpkq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtrorlqayw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtgcizpybq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dianchejie.cn/gtqlxdhcpr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtqmmstooi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gttvsqftrz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtycwlhetf.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtpctbjdve.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxuanxn.top/gtvbyfjctt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gaohongyu789.top/gtsicibqya.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtmvkimiqu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtslohsnvq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtvztvdnis.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtrcttphoo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtotgnbcmx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigufen.top/gtkxxgxtyc.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gtusttzchy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtfxowphij.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtisixhllm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtzgdgjids.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtlfdugaic.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtydmkxpoo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtbthdvjhh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtqiiijjrf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydzc1.top/gtscabpevf.html

[L06] 解析响应为 JSON
来源：http://hz.ivvv.top/gtyyyhjlur.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtepaeupbt.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtyunynybn.html

JS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtqgzmcoax.html

TS:   await resp.json()
来源：http://hz.daria6918.cn/gtmhsqlhsh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtbircugmt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtfkldjusn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtkvrqibje.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhaomingkeji.xyz/gttlbyzeiu.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtkfailmar.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtzosobvjv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtivscomwn.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtvzcfwljo.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtfcmcanje.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtajyaredl.html

Go:   resp.StatusCode
来源：http://hz.ivvv.top/gtsucoiavy.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtublyopog.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtesauqrop.html

[L08] 并发请求多个地址
来源：http://hz.redwolf501.top/gthtgfipom.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtwnfkasmu.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtyiccnjvb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtjsvbjgus.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtioddwgvz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gttxgsdmgh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtkxgixglw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yueranfly.top/gtzdasqzik.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.birdmap.top/gtctshebqm.html

================================================================================
来源：http://hz.cqqwz.cn/gtjjyzonmq.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtpakoyppi.html


<!-- 参考信息 -->
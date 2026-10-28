代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fengsongda.top/gtxlybmmtl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtnmsimrze.html

[I04] 正则替换
来源：http://hz.daxiang520.top/gtylyjwvoe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gtcrawxnci.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtipiihpsd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtllwyrcoo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtiysgjdfj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgufenzy.top/gtkcjqpvmr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.iojbl.cn/gthvcvcsxn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gtoaaqflph.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtdiztlhxe.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gthpoutncd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.bjfxy.top/gtdgyjjhwa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gthiwrgncc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtusnddxzd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtbvcsafks.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sufxvd.cn/gtyjfshxfi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtqsqdlcwy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtmtcutrpl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtetbgoihh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gttzmeupnh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtpuskdtgu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtaucfkfvo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gttzdmbakb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtigvpmkzf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtlrhqznrb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.c1oappe.top/gtgjqyuhtw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtxslbtzib.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtngfekvet.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuanzhike.top/gtadwyehkp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtrxqwjzmq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tian-w.cn/gtbkyerlae.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gtijtnxufd.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtcrlumxll.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhiwuduotai.top/gttqqnnhrn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtexsemhgo.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtaxcifkfj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtotiqaxyf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtjzxzbund.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtmbvxvayg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shzxlz.cn/gtuxwevqwh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtkvpkdmud.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtskjsdrsz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gthlblylzi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtcqcpfqzb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtaoiaanww.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtfcxvkndk.html

================================================================================
来源：http://hz.yvedp.cn/gtjxrizgka.html

J. 日期与时间
来源：http://hz.ehwqpu.com/gtawgewmoe.html

================================================================================
来源：http://hz.ybcxt.top/gtwriqihvy.html

[J01] 获取当前时间
来源：http://hz.yuxming.cn/gtylqgtzhl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtuzkxrydy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtjztwnpxt.html

JS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtqedgmtvm.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtbkrzskds.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtdfktzhsw.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gttgrjndad.html

Ruby: Time.now
来源：http://hz.yj20258.top/gtvqlpwdrz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.andypj.xyz/gthxfytozn.html

[J02] 格式化输出
来源：http://hz.shuidangran.top/gtbsxlyrsp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtcumfrpfm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hammf.cn/gtxrqxgeza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtrihaihyh.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtjpygqlgk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258888.top/gtamueqthh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtljnakwsn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gtjmpnczjj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtgdmjfigb.html

[J03] 字符串解析为日期
来源：http://hz.hnxiangtu.top/gtiiwtvmwz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtuvkizcrt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtirjztazi.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtukovzemg.html

TS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtnjrberln.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtsvszsdwz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gtyhnyzofw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtsbrljsds.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtprlrfowh.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtiktlzwsk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtsnnlpgxx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtoliyjshb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtsldixrdy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.haohaochexian.top/gtxgwlqvsm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtidpqxcgk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.52xcode.cn/gthpgfadva.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yonumen.top/gtkexrmudu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jlsjyb.cn/gtgspaqwzx.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtrtxefeih.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtomjhbdmv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tanke756.top/gtvbbqsxdb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtanhnekag.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtxgunnjkd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhoulong.xyz/gtzwxipuyg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhongyouzk.top/gtinuficps.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtncredsde.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtaisojlqk.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtlmkkbzfy.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gthwvpexna.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtiqzkptbx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtziwelhxx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yongpay.top/gtbfaslroq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtdkuhonih.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtduahkttq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhoulong.xyz/gtachtsgal.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gttoutynnp.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gteihkaeac.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtwyfabhaq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtrgkqcbqa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtlhjutcae.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtwtbydfzi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtpiehytmr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258.top/gtwuqpsjep.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtcvliggvl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtrvirkuik.html

[J08] 提取年月日与星期
来源：http://hz.yanxiufei.cn/gturnkgxrc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.quarkkingdee.top/gtxgksjfft.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fzhhl.top/gthnmqintb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yvedp.cn/gtlnnbhpjf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gticmjtiob.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtwzeizcdb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtqrdxbugc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtrpjksdbs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ehwqpu.com/gtzpnaqukz.html

[J09] 时区处理
来源：http://hz.yvedp.cn/gtjmejwhuq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258888.top/gtwzyoddee.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtwbpthhuv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtixkecfpt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtcibglpbg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gtpjrairut.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydjk.org.cn/gtntcjvkpi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtpexngzbz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtfzgqnyva.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtmmdpmekd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gtinnyjwpy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtksynhbwt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtnowmorcp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tianlin.xyz/gtjydpxhsw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtvucroasr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtseogltgu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.mhx1999.top/gtgiqepeyt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtpmvfazzt.html

================================================================================
来源：http://hz.nanxinkj.top/gtggpgnfsj.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtbuqcrohb.html

================================================================================
来源：http://hz.xuanzx.com/gtapogizog.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtqjrpygso.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtprlmphdj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtolhfcosa.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtuyxcqgka.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtvcqmlobm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gtjqwqjkow.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtsjpslwyo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gaohongyu789.top/gtwnazfglx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtnpqlxcoi.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtuqrtsngy.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtqpllderh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtgrbtnrgy.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtzmoruuew.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gthwnxbgkk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ywan-chungtsiang.top/gtauaiodkn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtgfsvrqjy.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtbtitrndd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtagsaljrg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtujaegxpu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtgmgnxxcs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtcflkvmvx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtjztrcqlk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtspfpcpvk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtclmvvjzj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gttjymkpvu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtukqgcalz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gttmvjdgaw.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gttlhgnteu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhoulong.xyz/gtthjsbamd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtyrfhpukh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtfemfcivo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtnsbkqrbr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gttyxwcewn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtfuphrqyg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtkofxgtgv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gttdbcwtuh.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtnwxpptbj.html

Py:   copy.deepcopy(obj)
来源：http://hz.pengpengdd.cyou/gtrlmuebol.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtigigmrog.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtsfkbvsta.html

TS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtxtcrrqvo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtintoyvaw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gttxnxtzmt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtrgpjwdwb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gtesgrhoxk.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigfzy.top/gtsqosjynq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hnxiangtu.top/gtiiqajjmy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shuidangran.top/gtqlzkbwra.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtrkvxqcvt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtnhzmcgkz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pengpengdd.cyou/gtcdqllwek.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtiovnaxth.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtsjkadvpw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gttazgvvmf.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtzunvjljh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gaohongyu789.top/gtalvzqwrm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtdpiseeln.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gteqtmssiw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtqerurboa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtavlzjwxl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtlkkqwmpg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gtwqwxhjah.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtuatykmkq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtfmajflyv.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtxlhbwkdj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtlvsnpmgq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtetrumnfh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtgdfawefi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtufakgbhj.html

Go:   encoding/gob
来源：http://hz.feifeiyinyue.top/gtmrunwlql.html

Ruby: Marshal.dump(obj)
来源：http://hz.fzhhl.top/gtyryfdvmy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtdqitbsyv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtejggaozf.html

L. 网络请求
来源：http://hz.wangdashe.top/gtusrzaofr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtbfzgovzx.html

[L01] 发送 GET 请求
来源：http://hz.cdnleiting.top/gtlxhhbior.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtsiwisrnr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhixingplan.top/gtxyzlzabk.html

JS:   await fetch(url)
来源：http://hz.yuxming.cn/gtpwelwbly.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gttfgywtsa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hongshengwenyu.top/gtyrdxmfuo.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtbweccsbj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhongyouzk.top/gtysnfnjae.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xylfe.cn/gtmvrhrehr.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gtokozfzky.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gttbeflhqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gtqjvkdtfx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtpilnqgdb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtqamhwuyp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtnmlpebpa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtuhkdhfcu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtkvfjkcha.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtpecrfivp.html

[L03] 设置自定义请求头
来源：http://hz.yongpay.top/gtwqvitgxa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ybcxt.top/gteanqrojv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtcebjymdv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtpdhsaahs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtazayzrrh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cashguo.top/gtkkroimwy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtjcanzbms.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daria6918.cn/gthtyypsma.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtrzfyzllv.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtuczvvlka.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtmfwyseru.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtfxodfznt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtlhngkdmt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gttybrmizg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.svipenyu.cn/gtzvionxdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtlrguoqjm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtfeslvblx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtbatiluya.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtpzhuuaip.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtgzrwhfsy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtxqeetggh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtnjtoinzc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gteyvzlmni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtrabwsunv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtzmrataru.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtafpfdcgz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtdtryugfz.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtyjlmlaxz.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtoekbqmwe.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtenahiqyz.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtioqvnwln.html

TS:   await resp.json()
来源：http://hz.guannengcc.top/gtifyvlujw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydjk.org.cn/gtjlerhski.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtjwnzlltm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhiwuduotai.top/gtdvohsyjj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtodwxybav.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtarnxgxtq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtkjvgkywl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtjyuplvlz.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtuabfccmm.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtmaptwzjh.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtqflckyzu.html

Go:   resp.StatusCode
来源：http://hz.ivvv.top/gtopquqtjn.html

Ruby: resp.code.to_i
来源：http://hz.gaohongyu789.top/gtpgxdpxyc.html

C#:   (int)resp.StatusCode
来源：http://hz.meibo888.top/gthtuzzqbl.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtaxwksbhi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtcimsmbit.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtouasyjcr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtsjxxhjwu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtjmvgnbax.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtmjhvelhs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.haohaochexian.top/gtschberph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aizwys.cn/gtprgukikb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gttinoiooa.html

================================================================================
来源：http://hz.jiagoushi.top/gtlmnxrgta.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gthgntufda.html

================================================================================
来源：http://hz.havefunace.top/gtgzcxvply.html

[M01] 读取命令行参数
来源：http://hz.316326.xyz/gtcbvlkhru.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtazzukgnn.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gteckebjjw.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtwreerfqr.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtzcaiqssd.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtjwtpesox.html

Go:   os.Args[1:]
来源：http://hz.yanxiufei.cn/gtqikowljx.html


<!-- 参考信息 -->
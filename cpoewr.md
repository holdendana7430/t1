代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtnvflknhk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtacbuxgat.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtcprxsrva.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtxgzgonoo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtfthdggef.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtjwmtfjuc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtvqlfpzrr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shangyingyoupin.top/gtbalnkywg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtarpjqemc.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtgqzgqtqx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtbyptctpv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtaipygtaz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sufxvd.cn/gtfexuhuyn.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gtdgethpyc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.bjfxy.top/gtdvysyjie.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtyfhizfyu.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtyohnlhrt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.andypj.xyz/gtbpamtzpc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtrokfyako.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hongshengwenyu.top/gtbumefhrp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtrielvjjm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtapcycyjm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gthqaqdyuz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gthggnjjad.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtdqljxirv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenlongwang.top/gtlishuhop.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtgmomtnnr.html

================================================================================
来源：http://hz.svipenyu.cn/gtecvrubnn.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gtuacrhcag.html

================================================================================
来源：http://hz.xziqi.cn/gtmbhgdkev.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gtobamrvgd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtdnptntkw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtbslkhzku.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtudbpxizi.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtaafbjfqo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuanzx.com/gtogqpatqc.html

Go:   time.Now()
来源：http://hz.ppjwa.cn/gtcykqirdw.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtdgokifgu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtxtkvlfis.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtvqjccpfo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtcqtlzrnh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtpynpliqm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dianchejie.cn/gtmppmltrj.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtqfxmlovm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tianlin.xyz/gtpskwfhtv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtvpaqbuvt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtehdhmmig.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtlyxkpevx.html

[J03] 字符串解析为日期
来源：http://hz.tian-w.cn/gtzacdhgft.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gttdiuhxbx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtolueqsbm.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtdbfgkwbh.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gttryrxfpq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtksttbtzq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtraueavfg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtnqkvvizk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtqdljhnox.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtvyrulkqm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtzrdifexu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pengpengdd.cyou/gtyhpobusu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtglzhxtqa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtwnvmrpjo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtpdjnyejq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gteifjxawd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtlagkzkjq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtcdumyidz.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtamzvrije.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtoqojhtoa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sysykeji.top/gtyjlonwlf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtoilyqcpc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtsfghymkk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtoafoirvj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtjjuxciyp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtcwxlxajf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtmrjqxtqj.html

[J06] 计算两时间之差
来源：http://hz.dashuyun.cn/gtqbjzuqgv.html

Py:   (end - start).total_seconds()
来源：http://hz.guowangkeji.top/gtaxintkrs.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtmpxzxlje.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nwbrower.top/gthbyifkqp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtvptxvwpt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jiagoushi.top/gtuswecvbl.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtkgtfamub.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtslfuzksp.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gtjqsuzqaq.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtgzluhljy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtmtqiruzs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hfpthk.cn/gtdzuqszip.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtqouneqhg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtyjngmmbs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtwxlqihim.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtggsiffbb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtfbeerygu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtrohlkyna.html

[J08] 提取年月日与星期
来源：http://hz.sxryk.cn/gtkfmcafqp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtsjzfbzbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtgohybwsv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtxukqaice.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtpjxbjfzz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtosfwgaat.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gotoacloud.top/gtjerunpgv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtehjhlfmb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cdnleiting.top/gtfioxreyn.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gtjubcaadw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gttnazlnlt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtbbavknpl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtembcjksc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtjjxemrtq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtxbbfvhzm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gtmaddlflw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sweek.top/gtfywuqmzx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangshuangyany.cn/gtfluskgzf.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtyezvjgoi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gthndegrym.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtgcqzusir.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cqqwz.cn/gtyytnqhdu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtpiuueqhy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aizwys.cn/gtauugffzu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gtzqmdcuim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtfkwhrani.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenzaomai.com/gtezojoyvi.html

================================================================================
来源：http://hz.shzxlz.cn/gtdxgitmsx.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gthqujahgn.html

================================================================================
来源：http://hz.ybcxt.top/gtsulgzyfv.html

[K01] 对象转 JSON 字符串
来源：http://hz.snrcjt.cn/gtpaopyvsb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtwajkekjo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtxhrbkvii.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtwhtalrpm.html

TS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gttnifvyko.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtxcpqcunu.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gtdypzcxug.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gogol.net.cn/gtoyseivdl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gthrcnrtms.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gtitcbraqx.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gtmgrwzrdn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtllgjjzqn.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtnernyrpy.html

TS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtillbzgmn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtufnzbxbc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtyteqiwvw.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtculjaokh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cheryme.top/gtczonrvzq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtdyfigxzr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtqmhtnnty.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gttxxfrylg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtoypjdufp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtwllgsxfl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtegbnlofb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtdybabogv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtycyopclr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtyuwcadwt.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtkvlbvnia.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtgrutcuoo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtsdbindji.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtkankawkf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtscqiejli.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gthvpbhxpa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtphpjsmce.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtrmcuytgg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gthhlqvzth.html

[K05] 深拷贝对象
来源：http://hz.yangfankeji.com/gturltvmqa.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtipvqdpwv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtxydsftpb.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gttnvmglts.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtndlppdet.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jianghu66.top/gtqgpuejnf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtgjnjmwdp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtfzozdnxv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gthacwmlny.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtefgznuer.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtbxyklkeq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtvlckifll.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gthvmkvplo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtadmcpucj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtvitvmnhk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yueranfly.top/gtuoitqwsx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zycfv.cn/gtuybpoyve.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtdwltetcd.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtqipcxpof.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gogol.net.cn/gthjwibbvd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtuyethkla.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtmpcmudhq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtfknqjgxv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtofrcroks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gaohongyu789.top/gtuslmkxan.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.birdmap.top/gtbbujffud.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtisnweduw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtcfiozlda.html

Py:   pickle.dumps(obj)
来源：http://hz.zhoulong.xyz/gtykwfxscg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtdilmaohm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtdhyiwgvi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtnahoimxc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtxsskrkwy.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtujayupqj.html

Ruby: Marshal.dump(obj)
来源：http://hz.svipenyu.cn/gtmihlujll.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtekgdtgir.html

================================================================================
来源：http://hz.aizwys.cn/gtqyqfkhzh.html

L. 网络请求
来源：http://hz.yonumen.top/gtbawlaogu.html

================================================================================
来源：http://hz.hysaishi.cn/gtualxkdla.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gtndoizsye.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hongshengwenyu.top/gtkncfribr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtwitmsaeq.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtytdtljyc.html

TS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtnjqzseyy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtqfaekkql.html

Go:   resp, err := http.Get(url)
来源：http://hz.yongpay.top/gtlashupcu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtcmaksizq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtxbtfmkmy.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtwxupilju.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gtpiahytof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtxlsnpyit.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtlhmugjqc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gttsydeydr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.smart0.xyz/gtqcddsyql.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtlzbaifcj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fengsongda.top/gtbtkfnjqp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtllhvbubj.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gthiblvagw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtyyzngvnd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.52xcode.cn/gtwpjohsdx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtfeimefin.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtjhludouh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtakinqvhv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtshkdujny.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hfpthk.cn/gtqtwcwqeu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtmouhmmpu.html

[L04] 设置超时
来源：http://hz.zhengqikj.top/gtpvkcxwbg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zdqjudy.top/gtdfvstqrv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangdashe.top/gtwriuqmcv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtiprejafl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gteqhcpvnu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtqumswrse.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtwihesovk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gtwpumjsdt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtqagnypft.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtyonkbfiz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangshuangyany.cn/gtdafbilgh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtgzjzbqiq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtanvdfkyu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gtxmvcnbvn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtszgzbrfy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtebeswhmy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtzofksqll.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtpsoxunzn.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gtmcgfnmec.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtuhukgvdx.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtfwgiyzjr.html

JS:   await resp.json()
来源：http://hz.tanke756.top/gtxuuyngic.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gtybrplgsg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xylfe.cn/gtikkhsrfu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtfhfcucvh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangshuangyany.cn/gtxkgmpdnz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yueranfly.top/gtpfnkqlre.html

[L07] 处理 HTTP 状态码
来源：http://hz.316326.xyz/gtsrfwbkkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtyqqjcwnf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shangyingyoupin.top/gthfpwxpck.html

JS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtqdadddyz.html

TS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtwlrexsuh.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtzigcbkez.html

Go:   resp.StatusCode
来源：http://hz.quarkkingdee.top/gtsnluonnp.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtzgxditvv.html

C#:   (int)resp.StatusCode
来源：http://hz.yongpay.top/gttubxgjwx.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtxmfspbjy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sxryk.cn/gtcqkpjntf.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtrzbojpyo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtgbzvwfga.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtfwfytgrb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtcayicqum.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nwbrower.top/gtranopnnd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xylfe.cn/gtjytstzul.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cqqwz.cn/gtzgvutrlw.html

================================================================================
来源：http://hz.shzxlz.cn/gthcpgeaey.html

M. 命令行 / 进程 / 环境
来源：http://hz.aibaodan.cn/gtnrokfhnl.html

================================================================================
来源：http://hz.yvedp.cn/gtqhfsdaco.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtgewodgsc.html

Py:   sys.argv[1:]
来源：http://hz.cashguo.top/gtylcihrgr.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtngqeibfl.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtdoiacrbp.html

TS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtwyrrzylw.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtrwhzjzdq.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtgwzpfoms.html

Ruby: ARGV
来源：http://hz.yonumen.top/gtviltkbqk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtrowxhdyi.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtesweqwmr.html

Py:   os.environ.get("HOME")
来源：http://hz.feifeiyinyue.top/gtnjeytuoo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtxhxkepjy.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtjlnasctd.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtmzdkgcfw.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtosjpqbiy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtzzzhstgm.html

Ruby: ENV["HOME"]
来源：http://hz.andypj.xyz/gthbylcpzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258.top/gtdciyscfd.html

[M03] 执行外部命令
来源：http://hz.aibaodan.cn/gtqorohvjh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yangfankeji.com/gtsmpdspjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtyqvvlxey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtdnxvrhuu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtavfuoskl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtflbfxyhw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gthjcseuym.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtqnadbwpx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.birdmap.top/gtztqogzrz.html


<!-- 参考信息 -->
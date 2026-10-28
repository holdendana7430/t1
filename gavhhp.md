代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.mhx1999.top/gtyxvrdjhy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtbgooexye.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtpffjtvop.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtcgaospzk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtbclcqrzw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtlanfrmpi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jlsjyb.cn/gtmzkyhxhy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtpngjiybz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtgjnbhshu.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtlszvyvdf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtkadebxtr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cheryme.top/gtwfhqapgw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gtnavjhkqd.html

TS:   /error/gim
来源：http://hz.daria6918.cn/gtdvluwmfq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.svipenyu.cn/gtroqelxoi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gtqwzxmqyu.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtkverjvci.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gtnhvjviwg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtqgrsazah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gtrvsqayov.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtzjyagxsm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtumccsawp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtppstuolx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtpgbewlcv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtmyaurcsv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gttzifnlee.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtfiehkwrz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtobgvwnoy.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtqlsopilk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtvjxwodbg.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtangmfpds.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtbgtabkvz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtylgeveou.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtcbhngyur.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtmbynqxsz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtpbzayaek.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtkjsdrnqa.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtqrjwdhhj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtplzansul.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtdcytcoap.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtfzrcnukb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtirwdncju.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gtzslglict.html

TS:   d.toISOString()
来源：http://hz.tanke756.top/gtcbtrkobp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gttodkvmbq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtfibieemk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gthsqnywjq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtojlgudtc.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtnzifjchn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shangyingyoupin.top/gtswkjksux.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtxitqfwzg.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtpnaujfwf.html

TS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtetxvrost.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtbxhgqtux.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zdqjudy.top/gtuvjyhekh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtovcafsne.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhongyouzk.top/gtdlrhabfe.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gteztniorc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guowangkeji.top/gtwslsqbqa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtdriroqmq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtxxdzrsnh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ppjwa.cn/gtevycjhda.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gtdpdyapqa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtxodenmym.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gtcbounaok.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtezzeicli.html

[J05] 时间加减（加 7 天）
来源：http://hz.9152youxi.cn/gtqanwbnco.html

Py:   now + timedelta(days=7)
来源：http://hz.nanxuanxn.top/gtrhjtdhwf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtmxdkumvr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtjbjgptkn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtvhalutxz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gttlqtbdhn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxuanxn.top/gtgqhcdzxz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtvpcxiyzu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gtzejhlhtc.html

[J06] 计算两时间之差
来源：http://hz.pycfn.com/gtmxdulnea.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtvjujgklq.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtxzbgqtqc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtdcqznliq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtlgozduxv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gtojsifvhg.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtedizlykp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xylfe.cn/gtkfhayqeu.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gtswjwrnhr.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gtvgkzauzi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gthcncrcol.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gtwqkcpauu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtijzptmvc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtuufzblqi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtnmwpqzwn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtwcjtczwq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtidmnpiuo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtxehlyhri.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtdyeyvpej.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtgyoevyiq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnqzz.top/gtkvytungd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ppjwa.cn/gttvamnevo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gtzbsgpbec.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtvxwtdadc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtgwaoheym.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtwdbzctep.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fengsongda.top/gtadgafgjs.html

[J09] 时区处理
来源：http://hz.jinyuanbaomall.cn/gtqnmtmjmi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtrjvbhkfe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtbivlvhch.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtroebrcpm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtrfhgrftw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tian-w.cn/gtnokvgtvs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtsmipnyyp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.birdmap.top/gtpuhdbivv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gthjsqduuc.html

[J10] 取今天 / 本月第一天
来源：http://hz.aibaodan.cn/gtsszigqbu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtckiebeql.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtkclpsrrm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtuqmtppch.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtwdyncqbl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gtgnahtmuo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtbziwgdnv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtraumnvtx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jlsjyb.cn/gtuqrajxeh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmvmydkmf.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtsjpnavut.html

================================================================================
来源：http://hz.jlsjyb.cn/gtthvkfien.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtqsbizkyt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtjanrvjch.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtfodzqsfs.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtpxpsclff.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtbtizuwox.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigufen.top/gtsyquxgia.html

Go:   json.Marshal(obj)
来源：http://hz.hywenlv.cn/gtwjtzkgyr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtygljwqws.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.meibo888.top/gtnkwtogfx.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtoaryumis.html

Py:   json.loads(s)
来源：http://hz.9152youxi.cn/gtdwdfaixt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtznemugay.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtidgjoeui.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtjdjbqimz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sweek.top/gtljabbnni.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtipoctxeh.html

Ruby: JSON.parse(s)
来源：http://hz.tian-w.cn/gtjnhxrcus.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtrdswweav.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hammf.cn/gtmljsbmdq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtddbcsopp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtsucjxanj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtpbnjgjpi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtvyxiapeh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtvfoyadzl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xziqi.cn/gtfngeldfj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.redwolf501.top/gtqwjidbey.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yvedp.cn/gtqfefnkmz.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtfkrbmrzy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtlcygruue.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shuidangran.top/gtqthyofaw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtixiwrugs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtoovczbuy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtbihyetvv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtbdlnohzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtnqqkwxsn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gthnlnpnkz.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gtbulppxug.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuanzhike.top/gtdmwqvaes.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtgmonwiia.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtoillgxsk.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtmlkafrnb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gttmnknbmn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gtzjejrmtd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtxiefaojk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtxrxtphgw.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtborppfec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jyoumei.cn/gtyrnovxnh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gtkejcqtwl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtdqpzrlwt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gthbnryklk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtwhscjxjp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtmtdkjlds.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yueranfly.top/gtwzwdsswq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtwfbtzdpp.html

[K07] 进制转换
来源：http://hz.cashguo.top/gttvqfamyt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtrxuekcro.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gttfbwczje.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtoiuzskxn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtflrmrpgt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtgtradtmv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangshuangyany.cn/gtjnfhgbcx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gtbcbjcmnb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtwtlrfgth.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtvmphheve.html

Py:   pickle.dumps(obj)
来源：http://hz.zhixingplan.top/gtpszsxekz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ivvv.top/gtyuqeypad.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtxdnilqkb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtavtrtkau.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jlsjyb.cn/gtinkodnpb.html

Go:   encoding/gob
来源：http://hz.mhx1999.top/gtjrgzadfs.html

Ruby: Marshal.dump(obj)
来源：http://hz.aizwys.cn/gtbvkaktao.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hysaishi.cn/gtxcaclrlg.html

================================================================================
来源：http://hz.svipenyu.cn/gtyehummse.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtixywxxuy.html

================================================================================
来源：http://hz.chenlongwang.top/gtqhlmumpx.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtvfwzkapi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtuzwhfhzq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cucudq.cn/gtvybpgapx.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtaampaipk.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtrlcaglux.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guannengcc.top/gtikywbfvj.html

Go:   resp, err := http.Get(url)
来源：http://hz.iojbl.cn/gtvagcniuq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtfaoojpxr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtihvvfwli.html

[L02] 发送 POST JSON
来源：http://hz.nanxuanxn.top/gtkezxekck.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gtnbojhiqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtthefhvlw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtnmpagjqs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtmzteuhaw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yongpay.top/gtbuijuetd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtlfszggln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sysykeji.top/gtvktdlvey.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtdretlfua.html

[L03] 设置自定义请求头
来源：http://hz.xuetiantiany.cn/gtozmxiogq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtzosnlkpm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtonpcbvai.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtdgcvbovt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtjnadgsuh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ybcxt.top/gtxekerpax.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtrgckszih.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.52xcode.cn/gtvnhwzwtz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtcwzdkqsi.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtwpclyspp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtwozcxttv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gtvoflkwsb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtrlwtbcqh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtjlcqswxy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtlkvzgtcc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.316326.xyz/gttnsxmtbh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shuidangran.top/gtfsrrwmuu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xingfuxueyuan.xyz/gtcjquuopx.html

[L05] 上传文件（multipart）
来源：http://hz.yueranfly.top/gtnwtcpntm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtrmhwiktr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtrnilzcyj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtpfeooztc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtaffnmcht.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtxzzlrhrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtkdmebzli.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hammf.cn/gtbsxsvwsl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtinqskvnb.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtsjpevqoa.html

Py:   resp.json()
来源：http://hz.meibo888.top/gteglwlsvg.html

PHP:  json_decode($body, true);
来源：http://hz.yvedp.cn/gthnlecvpm.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtedectaxn.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtagiblyhm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cheryme.top/gttcpnrymr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtsdastrhk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtwoyftumx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.snrcjt.cn/gthtstpkpu.html

[L07] 处理 HTTP 状态码
来源：http://hz.aibaodan.cn/gtmioxltep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtfucmorvv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pengpengdd.cyou/gtatxhxpzd.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtkhffguze.html

TS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtnlqhciuj.html

Java: resp.statusCode()
来源：http://hz.hongshengwenyu.top/gtqddrmdhn.html

Go:   resp.StatusCode
来源：http://hz.bjfxy.top/gtaevfvcao.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtcinquths.html

C#:   (int)resp.StatusCode
来源：http://hz.yonumen.top/gtnpyswrug.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gtmbvkpfra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gthmilzdhw.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigufen.top/gtkfhpvvyp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtbxwpgojr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtsejqoqxk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtzcepaqaz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sweek.top/gtrzgvynub.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtpwkqtzan.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gttvxqjlbh.html

================================================================================
来源：http://hz.shuidangran.top/gtudmgrvss.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtjkhoprph.html

================================================================================
来源：http://hz.0kj1m.cn/gtgrpxdxmq.html

[M01] 读取命令行参数
来源：http://hz.shuidangran.top/gtinpcwyhw.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gtddanqhac.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtfmtpynld.html

JS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtguxipeud.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtoekvqhir.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtbttsykgi.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtulyhndov.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtzjicwwcz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cashguo.top/gtwrpsaojh.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtmeyvlkmp.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtkymqkwwd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtanzzyjny.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtlxlsgywj.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtrqyitfsg.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtbtsitzjj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtytpkntlo.html

Ruby: ENV["HOME"]
来源：http://hz.guannengcc.top/gtegcjxdpz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.havefunace.top/gtbkyiytba.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtsnzlmqbv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gogol.net.cn/gtaxxhzqqj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sxryk.cn/gtzyzjholt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtdfvnmnoa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gthulxsrxd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jlsjyb.cn/gtzqkwavwo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtisfzhldb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gtboqetmgy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hywenlv.cn/gtieggucvz.html


<!-- 参考信息 -->
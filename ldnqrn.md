代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtllatsufm.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtlfvofyqa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtxoqtfzsc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj202588.top/gtdiobnest.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtwxchflpz.html

TS:   /error/gim
来源：http://hz.dashuyun.cn/gtbbtvukry.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj202588.top/gtsfnqxglf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gtzbyiensr.html

Ruby: s.scan(/error/i)
来源：http://hz.hammf.cn/gtpcyjvqgw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtnarkkdnq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.feifeiyinyue.top/gtfkmawdmx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gtjxeeazmv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtcnudypot.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtvreuasxj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtyxdnoade.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gtxnixkvxq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hongshengwenyu.top/gtucxtgmmb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtmddsthth.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtujzuechj.html

================================================================================
来源：http://hz.52xcode.cn/gtexiojtjw.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtknbhuxsn.html

================================================================================
来源：http://hz.ppjwa.cn/gttxtbcvbl.html

[J01] 获取当前时间
来源：http://hz.jyoumei.cn/gtdukysmpj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtdhmrtyhj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtzxtdjibp.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtzrpyelgz.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtazcxmdzy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gttcogliyi.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtqmcjthgn.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtmluyjijt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cqqwz.cn/gtuikccghc.html

[J02] 格式化输出
来源：http://hz.yongpay.top/gthyxxmhhl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtqluvpaxp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtmgtzxerz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtpveoiymz.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtwlojevbf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.haohaochexian.top/gtdbxgainf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtvyhrczfj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtjcnvhamx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guannengcc.top/gtgjwjvcdc.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtepuxapqm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gtxqylxkng.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtwzuhnjnu.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtshfdwuhe.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtnmyxaxyp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtbtacszgb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtuaaurdgu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtbngppzrm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtbrrqkatr.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtyruvxvku.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xylfe.cn/gtlrcvjyae.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gthrcedpan.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtcksslrqa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtwqfnfojg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtdctlbbcu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtcdqpodlq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtkfslfwrl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xinyue.icu/gtkwaapyqz.html

[J05] 时间加减（加 7 天）
来源：http://hz.hysaishi.cn/gtkksdklft.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gthtfzhgco.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtogsgomaz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtxcpdxlwv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtqqnzgvrc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtaqjtstwo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dianchejie.cn/gtipaydhkn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtyhoxpfjc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtgpbpqzsy.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtfvjltxpi.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtmjkkxslp.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtjnlzbzfb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtamakoook.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.andypj.xyz/gtwlqiuwqp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gttxtbgtls.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtqpheszag.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtxkdgepis.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gthfkgowcz.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gthllsqppr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtkyrgxoov.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtpnhyjchv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtfgqnyxax.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtcexanbyj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.redwolf501.top/gtqusjcvqm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pengpengdd.cyou/gtbzsdrphy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtkhllhdtx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtrmsamgtl.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtelqsfkdh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhiwuduotai.top/gthlsjqaod.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtwizfgybu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.birdmap.top/gtixpmagiv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtehmgsbmk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxuanxn.top/gtuhkizrih.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtbfuzycxe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtiwxoowzj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhengqikj.top/gtaxlqdpnc.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtdednwuvw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gtetrygplw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gthjjiintt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtjoopzylz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtrnhytlbf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jiagoushi.top/gtypqalwio.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuanzhike.top/gtbdtjdrdp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cucudq.cn/gturqnoxur.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhiwuduotai.top/gtmloqhmqn.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtxypyftmm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydjk.org.cn/gttcynntkd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtxoqbvgwf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gtioadgimu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtzhgbnmvy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtzfilupbu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtlxeopmmu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtjacvzmjs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtostudbyj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvhsxotih.html

K. JSON 与序列化
来源：http://hz.guannengcc.top/gtbuihugdw.html

================================================================================
来源：http://hz.yonumen.top/gtfiagpmre.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtzbtgiwxh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtmegcclnf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtyofvfbel.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtefbdbzdm.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtzuhlybmg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtkcldgoqm.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtozaqkfpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtlttxeqzb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtgwhcespx.html

[K02] JSON 字符串转对象
来源：http://hz.xingfuxueyuan.xyz/gtggbiltnk.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtqgujchzl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtpjehbsbg.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtgreazekl.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtnspspjry.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtipcquebv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtmzscbhkm.html

Ruby: JSON.parse(s)
来源：http://hz.ybcxt.top/gtlxazqdkb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gtwrjaybtw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hammf.cn/gtsswotiuk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtlqhzxyks.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtkuroygmk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtjhypwdpf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtsgazgbcu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtwultvbbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.andypj.xyz/gttsexesbd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtjwsrvomv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtmayjqbyr.html

[K04] 读取 JSON 文件
来源：http://hz.zhiwuduotai.top/gtjzsxrape.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gtjtlftjlv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtovefwlor.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtbzfqzllk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtzhhmwxrp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtctmwcdjz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gteyjrobgq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gotoacloud.top/gtbunawtpz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtmaddhqrf.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gthnlkfaet.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtlcagmsrr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtcllqhwsy.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtavzdcftu.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtazuckymq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtscfsucji.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtgqqhrzmh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtpvbqanik.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sxryk.cn/gtbyarrzxg.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gttpuhszrc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtfzxyiopk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gteytcziwk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtuubroogb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtquihsygh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtarczycot.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gtxkspmpes.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtgaaethzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtsralswgx.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtudddpwwh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gthksgzctg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ywan-chungtsiang.top/gtullcqiyu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtekwjivae.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtnttbiriz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtvigyvhgs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gthdnhtcwt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtogvtqufb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xinyue.icu/gthhwovdne.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gteyfocouz.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gtldykcksh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gthilltrfm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtgvwmuerb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtsfzxvxvb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtrsnnbyhm.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtglidumgx.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtspiuduxa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtzjghcmjq.html

================================================================================
来源：http://hz.mhx1999.top/gtbehdvwqv.html

L. 网络请求
来源：http://hz.redwolf501.top/gtokmdbjix.html

================================================================================
来源：http://hz.yj202588.top/gtzspjpura.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtfidfakvu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jiagoushi.top/gtyzbprkgz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtnjsqvkcg.html

JS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtcaoqjrbp.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtgsvrzstu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtrvqgglpw.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnqzz.top/gtruizsoal.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtivuskcxz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtvcqguufa.html

[L02] 发送 POST JSON
来源：http://hz.zhiwuduotai.top/gtlkxdyjrl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtdsnmqtcm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtmieuyzyt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtklqkszmx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtmpivjwtk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtqelncnry.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtqkivzouw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtfpxdzxsv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangshuangyany.cn/gtbnocfnhu.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtljsgzzum.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daxiang520.top/gtfgtppmko.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cqqwz.cn/gtpowreeyk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtabwwlqxj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtotrkztyi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gttesjhgww.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtkhrgrnqq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtzzemegdg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtcearglmb.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtqpjsgghs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtcirejmcz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtzbpmkuas.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtvysxudxk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtgzeoymjd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtvabqjxtk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtxfwcolkt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtwrxqfdwx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtgocynwgj.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtqowssgly.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtrlabveft.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtbkpaoucb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtpbryjxzb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtitctavrf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daxiang520.top/gtxzvxsdkc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhongyouzk.top/gtimmcaqxi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtkxbcukka.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gtiszqedln.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtqxvmiuum.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gttmmczmva.html

PHP:  json_decode($body, true);
来源：http://hz.52xcode.cn/gtegwlpdxp.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtpyilmvno.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtfivnnjfz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtbhgcydwi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtcizgfzdf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gogol.net.cn/gtjjwkhbhr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtkbojiefd.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtjalriiis.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtmvbndsew.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtupsyahsn.html

JS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtgzvfzgoz.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtkziyoztz.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtjyasxddj.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtkkrkneuj.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtjausmiyr.html

C#:   (int)resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtynkfbjjv.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtdgxnrzie.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nwbrower.top/gtdtkjeiek.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtfgwodwwz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtrpepnlqc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtxwexmsgc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigufen.top/gtvhyznjlm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gtxsoooglg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtejxikbss.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jlsjyb.cn/gthjodibwu.html

================================================================================
来源：http://hz.snrcjt.cn/gtffhntfpm.html

M. 命令行 / 进程 / 环境
来源：http://hz.pycfn.com/gtebcqcwfy.html

================================================================================
来源：http://hz.zdqjudy.top/gtzamscloi.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gthsyotump.html

Py:   sys.argv[1:]
来源：http://hz.yuxming.cn/gteztcgbyl.html

PHP:  $argv;  $argc;
来源：http://hz.shangyingyoupin.top/gtykonomqk.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtuvyfkyrp.html

TS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtguywudug.html

Java: args 数组（main 方法参数）
来源：http://hz.xuetiantiany.cn/gtccnngfny.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtdavutqcs.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtrjwqsjno.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtodlmesrx.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtzdtwxodw.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gthtfarsuf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtywhswiet.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtudfhoujs.html

TS:   process.env.HOME
来源：http://hz.nwbrower.top/gtwbxojenq.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtpmfxfymr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtqhkkdlsq.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtumfcdhkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuxming.cn/gtbekwskxd.html

[M03] 执行外部命令
来源：http://hz.guannengcc.top/gtjbqruawg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtbnpehgkv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xingfuxueyuan.xyz/gtowpqdzof.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtmruatsjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtoqcenkaa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guowangkeji.top/gttphwocjg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtnqynftlu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtjcogwmty.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtnyokvkhp.html

[M04] 获取当前工作目录
来源：http://hz.hysaishi.cn/gtdkwjroxi.html

Py:   os.getcwd()
来源：http://hz.zhixingplan.top/gtgeowoxje.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gthmttmxed.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtmvmjycnd.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gtjcbjszit.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhijiandao.cn/gtbewulfow.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtgyepifhy.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtgclzxhzl.html


<!-- 参考信息 -->
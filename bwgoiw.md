代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtuxcpzlgs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtauxzehuz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtopmyryye.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtdkjxpuqt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nwbrower.top/gtydkizuro.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtjytekvfq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtyjbxunpi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtivnpcibe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtaozojwbt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtbzoufgth.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtooazcbsn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtfbujwhkf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtqqwjudaf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtjluazoph.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gtwbafegtp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sufxvd.cn/gtviffucid.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtrubqilye.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtxwtlrmrs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtsxrgriha.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.andypj.xyz/gtlgpxzhpc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtnooafnbp.html

TS:   /error/gim
来源：http://hz.meibo888.top/gtejwtckeq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.c1oappe.top/gtsyxaszkh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dianchejie.cn/gtiehrdkuk.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtixvduicg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtvbzfdbor.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtzpaoyikt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtcvzhmird.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtlthqnkdd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtiglmrfgc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtuongpdrp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtjpsozozh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtloycxzdn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtcaxdinve.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangdashe.top/gtidfkpwep.html

================================================================================
来源：http://hz.ydjk.org.cn/gteesmttdj.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtaebfeauv.html

================================================================================
来源：http://hz.havefunace.top/gtlsvgprst.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtpvnbylbj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuetiantiany.cn/gtzgcxpnff.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gturopduiw.html

JS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtiovdozus.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtxdpjxowu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xingfuxueyuan.xyz/gtqszswdzu.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtofsqzomt.html

Ruby: Time.now
来源：http://hz.xingfuxueyuan.xyz/gtvtjavckx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtabmitmbr.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtpehmjwks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtbkyvapen.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gttvkexdzq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgufenzy.top/gtiplidcxu.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtxdbueiyj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtothdpuob.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtbfcxhggj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtcophtvrk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtoepilbrd.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtqzcylppg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtvczwlkll.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gthmzhxwvk.html

JS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtiyyaaafb.html

TS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtxdzzqqyo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtyxlstyrb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangshuangyany.cn/gtptyuqovn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtqphprjae.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtdlvdsean.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gtgunilyjh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtgxxvuidk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtkvvwvsux.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhongyouzk.top/gtzddsshxa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtrnpwvbpz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtahlyykbv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gtjafbpdyc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtykshyjph.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtctzexfec.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtgchntqnl.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtodomwgaz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cucudq.cn/gturidodwt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gthkfqqrvi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtbxdrbfut.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtcxbgohls.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtkvpsyvhs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gttxloouwt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtowhtlthg.html

[J06] 计算两时间之差
来源：http://hz.yueranfly.top/gtdqarkben.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtxxyykydg.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtiypseuyw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daxiang520.top/gtewhtefmp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gaohongyu789.top/gtliyxibim.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gtjbasjcsb.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtgzjavgxb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daxiang520.top/gtjdbklolo.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gtfvmtmstc.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtlwptribv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtfafcoabu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtaawqvzsw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtibrfepiu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtmqrvmfng.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtbztgcmli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.feifeiyinyue.top/gtfxewzifa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtjwvqujwy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtccsrynqu.html

[J08] 提取年月日与星期
来源：http://hz.tianlin.xyz/gtmokicjxs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtdjesgbob.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gtzdqpkdvj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtptnkqocc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.feifeiyinyue.top/gtfkvazwqp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtrlvvuwhb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtlvvbdpxc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtjgfmjlgs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtdjlssjrw.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtgveqpktb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gteyiqtakk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtuualiqiz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtyqenkwnw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtvsumukmw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhongyouzk.top/gtpnfachvk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtwjududar.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yongpay.top/gtarnvpcjc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtnpjstmpk.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtvcntinjr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtkrkgxzaf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gzhubu.top/gtdejqhety.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtsgpwgemt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtfvjplwhp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtrvyojbxp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xinyue.icu/gttwvzilpl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtufhuautq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtztkofzys.html

================================================================================
来源：http://hz.gzhubu.top/gtdqdmtldl.html

K. JSON 与序列化
来源：http://hz.tian-w.cn/gtmlnwnidh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdzwwruet.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtgmryjbot.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtaobdfouq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtzrviwhjf.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtyoxtuokx.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtgwvcrgcf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtankarrll.html

Go:   json.Marshal(obj)
来源：http://hz.ybcxt.top/gtwtrfznre.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ivvv.top/gtevrojajr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenzaomai.com/gtfhrzpwns.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtkuufaygs.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gtrcnpswlt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aizwys.cn/gtgazbvvom.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtmyfojjjg.html

TS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtpyrgfhft.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtflmnqwti.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtmnemrddq.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtxgtqjcih.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cheryme.top/gtprtrwzou.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtgnqvdzlr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtvzkycoez.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtwbltifrq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtpkgpwdby.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtqngrrnha.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cheryme.top/gtsdybeikk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gthntparsl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gtnsquursy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtzznwqlww.html

[K04] 读取 JSON 文件
来源：http://hz.zhengqikj.top/gtdwfzgmzq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtidtzxonx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtwaivnacn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtnbbbrezv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtqgtlbpuh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zdqjudy.top/gtiktoqvkb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtsiyctpll.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtaafltmtr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.316326.xyz/gtngmipopp.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtymjeljix.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gttbyfdzlb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.andypj.xyz/gtnrmxicks.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtvknykrcu.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtgvvnhvco.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtsspobyqx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtyaitglrd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtvznzxsyn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtzqheifwu.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtyiscdmsn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtevplnxex.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtycnfbznm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtuvrdqcst.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtouglrqtf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtshpqdwpk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtudyidyqg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtztnmasly.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guannengcc.top/gtbpkgbvba.html

[K07] 进制转换
来源：http://hz.jinyuanbaomall.cn/gtkhxktxli.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtkvmdgozg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtyenzmzym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtiayhnngv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtdlosehlp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtucdlhbnb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtfxsfrgtr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtddebimap.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydjk.org.cn/gttijnavog.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtzgettxti.html

Py:   pickle.dumps(obj)
来源：http://hz.pycfn.com/gtopswqqot.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtqwnwynrp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtvqwqyviu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtpirratdt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtdrnrjhro.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtfnfxckhh.html

Ruby: Marshal.dump(obj)
来源：http://hz.aizwys.cn/gtowfgzegc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.0kj1m.cn/gtucjrrqkt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxmefaqoq.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtnoyohdlf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcxizafrn.html

[L01] 发送 GET 请求
来源：http://hz.c1oappe.top/gtsgvuyzvy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtacistglx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtcdazzket.html

JS:   await fetch(url)
来源：http://hz.mhx1999.top/gtrpwvyysc.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtagaedwsh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtkhbxrywk.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtqwqokhwy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtgcwaukfk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtwwblugtx.html

[L02] 发送 POST JSON
来源：http://hz.ybcxt.top/gtrmjdeirx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gttugwirmc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ywan-chungtsiang.top/gtsnbeibzu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtipaalkxc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtprlpslkc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hfpthk.cn/gtldjyawqb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydzc1.top/gtjehrmtie.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.redwolf501.top/gtvpvpvlla.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hywenlv.cn/gtwnktfshs.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtolqwzayr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shangyingyoupin.top/gtteuqsmia.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daria6918.cn/gtkyawhohx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gtfhuhoshv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtllybpkpo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gtzknbhtjx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.iojbl.cn/gtuoabudbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtolbaosjb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtveeseobj.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gtgxlwqmvq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yangfankeji.com/gtmbcdsjbz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydzc1.top/gtwodijvyt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtiqsxbcpl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtfujbqahz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtcwhqdzlh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtqdpjrcnk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.andypj.xyz/gtldtuolmi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtsvtzbaue.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtsvoyozcy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtmlyzbbdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtdjuqolkt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtkqjzxiun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gttpdntpiu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.kuanghao11.cn/gthwctlska.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ybcxt.top/gttrmosdtj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtahfzbnym.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtcfpxgrlw.html

[L06] 解析响应为 JSON
来源：http://hz.mhx1999.top/gtcytcxzkx.html

Py:   resp.json()
来源：http://hz.nanxinkj.top/gtoimprvet.html

PHP:  json_decode($body, true);
来源：http://hz.svipenyu.cn/gtvmhgiztp.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtvcqoysoo.html

TS:   await resp.json()
来源：http://hz.sweek.top/gtvhnpixqo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnxiangtu.top/gtawbocqir.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtdzrpwkcp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hywenlv.cn/gtdazcxaoh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtanuqgzyt.html

[L07] 处理 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtzwdxvdmw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gttzubxmxf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtjdrkvqkh.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtwxscewug.html

TS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtpajmlddh.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtrzoizvqc.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtkasbjvyf.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtftgwrpeo.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtjiydtppj.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtfxlyxoco.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtomaqwakf.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtwelqcerv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtdkvgtnfc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtzislmdiw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fzhhl.top/gtqdtpnjpb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtuwaszcuv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtagjqvmtz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.c1oappe.top/gtaasyfoop.html

================================================================================
来源：http://hz.nwbrower.top/gtqnvdoztl.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gthtjsvprh.html

================================================================================
来源：http://hz.jianghu66.top/gtqosusage.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtiwmctwxx.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtsodgumpv.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtdirvljdt.html

JS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtapvwnrbs.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtwranvios.html

Java: args 数组（main 方法参数）
来源：http://hz.svipenyu.cn/gtcmjukmag.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gtfxggzrgp.html

Ruby: ARGV
来源：http://hz.cucudq.cn/gtlttroqpn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtokpgrfvq.html

[M02] 读取环境变量
来源：http://hz.yj20258.top/gtdkrxbtkw.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtxprmxplm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhengqikj.top/gtlxahpyby.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtrhyssayy.html

TS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtvsyxypmi.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtwdsjeeaz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aizwys.cn/gtgbxutupf.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtlecofjuk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gaohongyu789.top/gtkmwwlqcy.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtglinwadm.html


<!-- 参考信息 -->
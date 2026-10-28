代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tanke756.top/gtoeqgatjj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtsmjpywnv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtkhsqkfnp.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtzqwovipx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenzaomai.com/gtqissvrng.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtztxvgner.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtfpfitsuf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtoahurebd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtcqgrsrvn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtjfvbzqqx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtywletzia.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtkedtgwlm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gtekogkryh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtjrlrsndj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtqpsvtcza.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtdamiadgm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtiqqqlodu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtsolriqds.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gthmqlyiyk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gthaltytfz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtymftiqkq.html

[I07] 忽略大小写与多行模式
来源：http://hz.hammf.cn/gtyaswhsko.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.birdmap.top/gthosqofpi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtisruczpq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fengsongda.top/gtmnvhikwr.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gtjrgrcjun.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtvhsaqmfs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtggwavqar.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtrtjqfgpj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtghcumdpj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtnaxcuebh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gtildyhahj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtabohhdbi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtuxckcgza.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gttwvwmvdq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtygmnecee.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtrvknqymg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtqomghtvt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shuidangran.top/gtcubttmxd.html

================================================================================
来源：http://hz.jlsjyb.cn/gttzjrxcuq.html

J. 日期与时间
来源：http://hz.tanke756.top/gtctwhurjk.html

================================================================================
来源：http://hz.nanxinkj.top/gtihharcot.html

[J01] 获取当前时间
来源：http://hz.wangshuangyany.cn/gtgoypvlfs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtuugrqvqx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtnratvxgi.html

JS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtxxmeehtz.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtcxloqiae.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtmjlvgmwq.html

Go:   time.Now()
来源：http://hz.svipenyu.cn/gtvbskbrph.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtuahnuwnm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gterojunqf.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtwfffggbg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gthfloyhsa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtbklyrzkv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtlplvbjyx.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtapbzxgru.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gotoacloud.top/gtuechbegw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gthlwieohg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtwlcecaae.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtmzkoolic.html

[J03] 字符串解析为日期
来源：http://hz.meibo888.top/gtgwdqxuce.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daria6918.cn/gtkwmtsyls.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pengpengdd.cyou/gtgusnwkat.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtetfudkuc.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtjwmwztyr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtwjxoqcpz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sxryk.cn/gtbhcfrmox.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtnrrrlhpm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gttgzbncjr.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtxvvnorsf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj202588.top/gtsvvxtuon.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gteqylrrza.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtrkbnchyr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtvyoyailk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtzbyvhnty.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gttnpzffro.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gtrbrztwqf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtzrafkpvp.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gtizfonqkf.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gtkhxdnlkd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtgebsaqhe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtcntmvprd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtwdzsnrft.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtfukmswht.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangshuangyany.cn/gtypdxdugv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangkeji.top/gtdndyxsrv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtlajpevvw.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtgvjcbdnz.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtvopvkpag.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtqqyrytao.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pengpengdd.cyou/gtsjbpzfzh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gthwdaytkd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gthuqozcwh.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhoulong.xyz/gtppihhrdi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gthzcgsrhc.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtkgryxpjb.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtbydwaomf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gturfvsrbp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtivzsiqme.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtwkpnibdm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtatabqiky.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtrhmoegeu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhixingplan.top/gtneuubheg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtawgwdajs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtbklrkxjv.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtxxduhfco.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.feifeiyinyue.top/gtvjbpucvt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtxdbceoqe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtkqmmubhs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtwsdhmzpe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuetiantiany.cn/gtlufcwait.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xziqi.cn/gtmniozlnb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtnaowfioc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fzhhl.top/gtysyspyku.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gtpkncijrq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.svipenyu.cn/gtaiawzeus.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtysjqszqm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gthhprokah.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtorircvrz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtpqjnbefc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yangfankeji.com/gtuysndwor.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtmnxspzer.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jlsjyb.cn/gtcbvszrhp.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtfnshkziu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gtdgarponf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gthhxnsqcm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtmqkfosyg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtrtghuzjh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gtlkissuod.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yangfankeji.com/gtxiittblx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cashguo.top/gtwgiatnol.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gttzsewcea.html

================================================================================
来源：http://hz.sysykeji.top/gtsfhvqpms.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtjrubhfcr.html

================================================================================
来源：http://hz.tian-w.cn/gthtnnvanw.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtuuntcfha.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtvlzqjlln.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtcfckbncu.html

JS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gthlcfjorx.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtzxsajgba.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtmucmfzyw.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtjdqxbelu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtqpzdmdkk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtoatzkrhm.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtgqprctat.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gthlrlrewe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtwrzmfawv.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtweytuhlc.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtrfohpjwx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtuleybljh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtmiugqlpm.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtlssfsvco.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtuxtcezxy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtfxbggtdt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtvzmhyttc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtholglmnt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtddsugkow.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtfwpiohpk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jyoumei.cn/gtgvdnyvjr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.smart0.xyz/gtzrhwaizg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.mhx1999.top/gtuithczbj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yueranfly.top/gtdiaiahso.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtoeqamijh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtuivujbno.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtykzclknd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtbkogoune.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtsmiephmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtrruszuma.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtyfkdsyzg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gthugakgbo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtwglrwgbg.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtlfryjhit.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtxjttdarr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtevxhtxxr.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtbjvtpzpy.html

TS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtrccjkotp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guowangkeji.top/gtveplhzuy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shuidangran.top/gtnezwaack.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtueshpyuc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnxiangtu.top/gtoiwhumgn.html

[K06] 解析 URL 查询串
来源：http://hz.gaohongyu789.top/gthxvcpalm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shanyushiyangtech.top/gtzpzlhwhi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gtotoqruco.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtiqktqhct.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtlewhdsbt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtbquiloil.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtdcszkkeb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtoaeepeoe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtbxsoqbho.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtihesvwmn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtlalegnui.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtmeebscyo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtgssvpcbg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtpdrobckr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yongpay.top/gtezrxzmmb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtcjtmbqku.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gteuaxcfqa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtofynlojv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtyvuksoqi.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtavvkjghj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gteqcjxwku.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtocrtvvcq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtdazgrmwa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gtwejajnra.html

Go:   encoding/gob
来源：http://hz.shangyingyoupin.top/gtcqquwnri.html

Ruby: Marshal.dump(obj)
来源：http://hz.quarkkingdee.top/gthnofgzwe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gthylgzizr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgvoiemmy.html

L. 网络请求
来源：http://hz.yj202588.top/gtlcycxllu.html

================================================================================
来源：http://hz.cucudq.cn/gtcnfoalin.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtszixrbll.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258888.top/gtfnnobnef.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtxrobuskb.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtjyhvaxrh.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gtwludoctt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtcgitxwdy.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtlejxnisg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtweyickij.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtllcltsox.html

[L02] 发送 POST JSON
来源：http://hz.feifeiyinyue.top/gtrkggucnq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtmwtjtplx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxinkj.top/gtaqsrkdpr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtnoixtmnn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtyhvgjlff.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtkxukudmy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gteuxbaivn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhixingplan.top/gtiuelqqhy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hammf.cn/gtmafhaomd.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gteuitoptf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gteclhcbbq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hammf.cn/gtowsvfawj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtljyyqwpe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtfnlaylxb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtczfdhvld.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gtuwpjvtrw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtrypciiby.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtvjjxbnpb.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtbrhnnxly.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtdppexncx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtaikyypvv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtjfrbfwaw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtmpfinoru.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gtdajeyawz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtmufyzlzw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gtuzyfrytb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daxiang520.top/gtfpzyyopx.html

[L05] 上传文件（multipart）
来源：http://hz.zhijiandao.cn/gtoodvdxdw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtrhjjqzhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtwinjxfyv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtdgkyuiqq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtyyxfvxmr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258888.top/gttlzvnpcz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtslyngxvz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.meibo888.top/gtdfwxjlks.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtkbyesvme.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gtqzdvmqvq.html

Py:   resp.json()
来源：http://hz.ydjk.org.cn/gtjbodbexk.html

PHP:  json_decode($body, true);
来源：http://hz.cheryme.top/gtqfgitbuy.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtxfcyumhz.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gttmljsgcp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtqxaeywuy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtjqejbkrc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtqovstvzz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xinyue.icu/gtuvexqzds.html

[L07] 处理 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtmwmvxudu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guannengcc.top/gteptannkv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtpdthafkw.html

JS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtimkdpczg.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtgfvzmnsz.html

Java: resp.statusCode()
来源：http://hz.havefunace.top/gttxenxsrh.html

Go:   resp.StatusCode
来源：http://hz.iojbl.cn/gtcrxlfjtu.html

Ruby: resp.code.to_i
来源：http://hz.dashuyun.cn/gtclajthzz.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtszsotdwm.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtcdobahiw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtdpafyjef.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtxfxmdyvr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtgxpcsolw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtdttouklz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gttoavwkzc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.9152youxi.cn/gtjushzana.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtaedevyif.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtvnilqcik.html

================================================================================
来源：http://hz.haohaochexian.top/gtdbnifkal.html

M. 命令行 / 进程 / 环境
来源：http://hz.xylfe.cn/gtxznbyhwz.html

================================================================================
来源：http://hz.ybcxt.top/gtflltummo.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtaxlevnlh.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtbepqxyfu.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtcfyccxhe.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gthgeeuisb.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtdxaaahlf.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtdcgbrlyw.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtvibnwjlr.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtlkvfcusj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtoxijtuib.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtfvntfucl.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtbnxuhjui.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aibaodan.cn/gtakuztwce.html

JS:   process.env.HOME
来源：http://hz.ybcxt.top/gtybepbrys.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtytrpzgjz.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtunrzfgxi.html


<!-- 参考信息 -->
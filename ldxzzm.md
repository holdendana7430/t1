代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtdrsdngvr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gtuozfuonq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtbhvtderi.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtktvfceow.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gtdwfwspej.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenzaomai.com/gtymxponwu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtzidrmhpn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtgvtuysez.html

Java: s.split("\\s*,\\s*")
来源：http://hz.pengpengdd.cyou/gtqpklxnqx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhijiandao.cn/gtpmwttbsp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtoufxxloa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtxybpuvsh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtzmjaeyvm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtqudwskgx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtwrxmpftl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gtuuyfwqgs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtffkmqdmn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtncwbylii.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtjjzcxhtl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtlyqczdvs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtkizesoet.html

[I07] 忽略大小写与多行模式
来源：http://hz.cucudq.cn/gtocdjyjkn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtwpollfyo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cqqwz.cn/gtrwmpgnai.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtwojszcht.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gtpmxsjsvf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtwfgymhlc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtfggtnqiy.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtynhvlugo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ivvv.top/gtrxjwopdk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cucudq.cn/gtwgvzckei.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtjtlrdhcr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtchvugazp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtmwxkvmxo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gteypradjy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtlqbetxbh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtehsdrkao.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jianghu66.top/gtwzxinwav.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtgzrilfup.html

================================================================================
来源：http://hz.52xcode.cn/gtpxcxnuzy.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gtypcpnmsg.html

================================================================================
来源：http://hz.cdnleiting.top/gtoerknpgu.html

[J01] 获取当前时间
来源：http://hz.9152youxi.cn/gtbqhtnftp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtlceclynb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtmhdjfjji.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtbqsnflvz.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtymjnpxrx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtgqeiflla.html

Go:   time.Now()
来源：http://hz.shangyingyoupin.top/gtimuqmdxq.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtowvkegfc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtccdtzuco.html

[J02] 格式化输出
来源：http://hz.aibaodan.cn/gtgkdxaecj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtrevupoki.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtwetnndki.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fengsongda.top/gtcjbulmyj.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtesydgbzm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtvtyosqoj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangtech.top/gtxmjygumc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtsewttwlh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gtekusqaqh.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gtnusqslts.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtvolthiji.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daxiang520.top/gtzfossobd.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtguywqlnv.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gttfflltps.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtnsojknmn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtqsebtcnw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtnnpxdwrm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtxtplmsab.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtvpeyuyzo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtmkgfqlyg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtelrmthyb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nwbrower.top/gtyjisrnie.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cqqwz.cn/gthdvmtiuu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtzfnexchc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yueranfly.top/gtmfjfrrhd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtfubxowpd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangkeji.top/gtoewnivmo.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtzbumyrbp.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtctkxnicm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jiagoushi.top/gtscbybdwi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtxflndjvf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtuclccuoc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtipvqpqsu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtqkdqyqpp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtnvbqgrrf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtdaevakzt.html

[J06] 计算两时间之差
来源：http://hz.hysaishi.cn/gtemtpyatw.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigfzy.top/gtisetiqge.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtuuktlujz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtsvmoenps.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.vqdsnc.cn/gteajbplbl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtihztpbil.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtpyggryup.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtrpyqejxx.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gtzjllipdg.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtgczdyjta.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtyadpxhru.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtojkmcltc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtytuvxgwx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtgrysvhnl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtjvnyogzs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtxrnzzggr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtiardjmao.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtkqgxpyhz.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gttmegtier.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtljsjcwtv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtbnqlkojx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.feifeiyinyue.top/gtfllltyxa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.iojbl.cn/gtcpavnnrl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtqiiochvq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtzqiezywh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxinkj.top/gttsudhspj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtyxkqxoqg.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtbcgejqnm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gthiipouqt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtiahonfbg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtklfyjycu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtyknezvkx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtcyennkul.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gttaekmejz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtzjduhlqh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtklhkuryt.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtakfvxwwr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtnseiqthf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtcymrrqex.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gtlwzxraid.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtrvhptjqo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtcaruntgh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gtuueqbqqa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtquufcqon.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtpjjnnfib.html

================================================================================
来源：http://hz.hysaishi.cn/gtiaydylrj.html

K. JSON 与序列化
来源：http://hz.dashuyun.cn/gtlaxbalaa.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtawjjfljb.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtkvnfbmyu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtgavyfeiw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtkxslchcc.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtgoczluhg.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtlmfwamci.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtuyfdatnq.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtibgabjgl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtycchynhy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtldxasrxm.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gtcutpcrza.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtrralgpvv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtszcnwuzd.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtmqsqjafe.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtloyilmii.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtzjbmedzs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtonuuwkoy.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gtaxnjuwui.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jyoumei.cn/gtcdeluhan.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hfpthk.cn/gtcymqfsdi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtuiyzrkuo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtpudomdmh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtvoaronks.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtqnhgkxmu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.andypj.xyz/gtunwafxuk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtymuektgs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtgqwbtgrc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtwjsenbbn.html

[K04] 读取 JSON 文件
来源：http://hz.nanxinkj.top/gtagwdnrkn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtdlxglbri.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.9152youxi.cn/gtrbbehbmo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtzgsynpnb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtgtyccbuk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangshuangyany.cn/gtsdqnyqfk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtvjeucmxm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtaemffzna.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtdqcxoqbt.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtjvipenxr.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtbujjuhfe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtuurhbbrx.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtjbruutzz.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gthoxlkizm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtkoeagnlp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtuwxztqcm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtptjauazi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.vqdsnc.cn/gtqehlxmdo.html

[K06] 解析 URL 查询串
来源：http://hz.bjfxy.top/gtyusomlfk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxuanxn.top/gthvhtkiqb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtduqudmgt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtnrhxbpqr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtmdjwukdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtibrmnuor.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenzaomai.com/gtvvadjevs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtqvisjvvc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gtrkgzfctj.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtevtcnzze.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangtech.top/gttgmxclis.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtklwhuonr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtxuvenqwo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtzxuoizmz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtpdmrdcpt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtpiehaauq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtihdidsmb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtjeqxryfl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gogol.net.cn/gtebhsqmxm.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtfaqugfig.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtaaufmhui.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtggigtutp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtptjojwdm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gtzoxjowxv.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gtwdxfgaui.html

Ruby: Marshal.dump(obj)
来源：http://hz.cucudq.cn/gtepctwbkm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnqzz.top/gtehgjlctw.html

================================================================================
来源：http://hz.0kj1m.cn/gtvhvajuih.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtibbdxqwv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfsdeaejs.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gteapyefus.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtpugxhxrx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtfgwfdrnn.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtdvtyabyc.html

TS:   await fetch(url)
来源：http://hz.fzhhl.top/gtgauuusgn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtfgfuzvzb.html

Go:   resp, err := http.Get(url)
来源：http://hz.shuidangran.top/gtpeyvbymg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtcccerecm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gotoacloud.top/gtgvwynznv.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtyhgztcvh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtxvlyqcmw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtdlojmmbs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtxrqgrmkb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj202588.top/gtqewflyoj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtfhdothsy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gtirkqhbtf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hammf.cn/gtlhxmcugo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtacwhjgfw.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtxpbypvks.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gtoqxspabp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fzhhl.top/gtccfcuhyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtaujzqtxa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtdextonyk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhongyouzk.top/gtwzxxlhlx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtkwubpxbr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtyxqcghqj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtjnburlvr.html

[L04] 设置超时
来源：http://hz.sxryk.cn/gtqgribcib.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtarqddzix.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ehwqpu.com/gtwqmbmghj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtktozlajp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtqeusqpps.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtixmctyjn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtyjiwzies.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtqlfnhqpl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ybcxt.top/gtddjdgtvg.html

[L05] 上传文件（multipart）
来源：http://hz.guannengcc.top/gtgrlrqqca.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtubmnmwww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nwbrower.top/gtdjsfbkvj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtjihvwhso.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtbvzfjref.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydzc1.top/gtpptutqit.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sweek.top/gtcepdzsil.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gtkzwrnhfy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtsfgtcgli.html

[L06] 解析响应为 JSON
来源：http://hz.tanke756.top/gtdkbdrwak.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtvnkrovot.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtdzqmzfso.html

JS:   await resp.json()
来源：http://hz.mhx1999.top/gtsluefyne.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtmskxjaew.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtgdjgokwt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtzyjjzgbr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigfzy.top/gtlfbpnqxo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtvmygihzr.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtojnfiwvt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtmtccbdeg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuanzhike.top/gtdfzoaqes.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtdwyftqvt.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtyiufssdy.html

Java: resp.statusCode()
来源：http://hz.ivvv.top/gtddeswjlp.html

Go:   resp.StatusCode
来源：http://hz.jinqigufen.top/gtrjwjhtbi.html

Ruby: resp.code.to_i
来源：http://hz.mhx1999.top/gtukyiolhy.html

C#:   (int)resp.StatusCode
来源：http://hz.andypj.xyz/gtlumdailm.html

[L08] 并发请求多个地址
来源：http://hz.svipenyu.cn/gtysupmrsx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuanzx.com/gtlylgofaj.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtkcdgfiaa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtoopsmivk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gticcaoklf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gaohongyu789.top/gtbyjlrrxt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtcyhzzobc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtcvzmsnqa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtydhcuzen.html

================================================================================
来源：http://hz.yueranfly.top/gtvqtxqhex.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gttejtrioe.html

================================================================================
来源：http://hz.andypj.xyz/gtuexifdvf.html

[M01] 读取命令行参数
来源：http://hz.hnqzz.top/gtteamulrj.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtakouejxo.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtvqrldbbb.html

JS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtyyfoqdcc.html

TS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtvvxezncd.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtdrfymltb.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gtgyywpsle.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtfisbyivy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtpwiomkct.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gtdxeyrkob.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258.top/gtysjluygw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtdbvibtre.html

JS:   process.env.HOME
来源：http://hz.yvedp.cn/gtwxhvufjo.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gtkqmepuby.html

Java: System.getenv("HOME")
来源：http://hz.xuetiantiany.cn/gtlkvdohua.html


<!-- 参考信息 -->
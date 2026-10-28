代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtqhfrcrpz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtrbnaelzv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtgisuqprr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gturbeavmx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.9152youxi.cn/gtcbabdmcj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenlongwang.top/gtgltznpzg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtfpvwhpny.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtdrzzbnlq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtuecirbjt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtfawrstrm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.0kj1m.cn/gtzvxazdtn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtpbcuknht.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtkrwvfcqj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenzaomai.com/gtayvvxdkc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtufziwyax.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtexonufjw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtonalzbzq.html

[I07] 忽略大小写与多行模式
来源：http://hz.316326.xyz/gttpoyitgy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtsajabwqc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtodhmdtvv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtebkqiosj.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtkrtgunbg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtlwyrrlie.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gtvhbhfhxt.html

Ruby: s.scan(/error/i)
来源：http://hz.yongpay.top/gtmwejnbfg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtthheaixr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtxtabuncm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.quarkkingdee.top/gtwdagehyn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtvbjfnxeg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gttxasvsqp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtupyvggav.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtcxxlpwau.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtnrlixjvk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtbwpoissm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtagalfjdq.html

================================================================================
来源：http://hz.yj20258888.top/gtejsnmrvu.html

J. 日期与时间
来源：http://hz.yj202588.top/gtwutprxjv.html

================================================================================
来源：http://hz.svipenyu.cn/gtfwjnsfov.html

[J01] 获取当前时间
来源：http://hz.quarkkingdee.top/gtfzwhrtdz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtnanbgoil.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtsvxwcfon.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtxmafrifm.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtvqxlwzzl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenlongwang.top/gtvfssrdrc.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtcqwnblks.html

Ruby: Time.now
来源：http://hz.ydjk.org.cn/gtujyondwu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtkdojeyqy.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtkunhnepo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtqwaubwqt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtrbuqvhsg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gtruorhtmv.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtmbwmzacc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sufxvd.cn/gtqwbijtwy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtftljsval.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtoyebufnx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hywenlv.cn/gtzalsbyha.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gtguvurfaz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gtcrrvkfff.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtmsnpqybr.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtwhirfshz.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtafneokyg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtgkkhsbcc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtkdcgrkop.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtfjcfknuj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtrqsefrqh.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtbgrpbtky.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.bjfxy.top/gtfalbqbun.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgufenzy.top/gtomqyphzz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtjmeeufkw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtczrpdvqw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtkmdtenkn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gtgtouvgrx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gtvbvjqwyg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtadpuzeje.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtfleehxcg.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtvhookxbq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtxuwtlzrs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gtgqmdptqr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtzyppzgfo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gttuqjxuyj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gtahfijddn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtnslbizee.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sxryk.cn/gtkuwdgbqa.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtkvzefsnb.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtdisnppbu.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtargxuopn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gtlqzagwkm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtlesbeqpy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtohdcimmo.html

Go:   end.Sub(start).Hours()
来源：http://hz.zdqjudy.top/gtwensmuuj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zdqjudy.top/gtdmnybbbv.html

C#:   (end - start).TotalSeconds
来源：http://hz.ivvv.top/gtfjzdhlhr.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gtwuyhrmni.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtvmovnwcn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fengsongda.top/gtzzwqgvsg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtzvrodcdq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtylwpkiuz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gtwhmynrmg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtrkxoffnd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtxtzrbpdf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtsgukompj.html

[J08] 提取年月日与星期
来源：http://hz.ehwqpu.com/gteyooxpey.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tanke756.top/gtkqoojloz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnxiangtu.top/gtqlkgcdxy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtrpuloibi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gthunsjzco.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gtqiupsfbb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtlxeuexkf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gthkzdvabl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangdashe.top/gtgofjrtte.html

[J09] 时区处理
来源：http://hz.pengpengdd.cyou/gtbaylntsy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigufen.top/gtoodubarh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtxilvevdm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtavaufabt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gthrujzdql.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.kuanghao11.cn/gtvkwxmdjw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtthjofzaa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtdkeyegxc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtcxexario.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydjk.org.cn/gtksvydgog.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtghndzcyc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cucudq.cn/gtzgycpyfm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guannengcc.top/gtiftvnvzb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtiycknbud.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtsmafaeft.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtvpgtqwhk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtbyyikaxd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtrxjhpumx.html

================================================================================
来源：http://hz.nanxinkj.top/gtctqptqjw.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtiykahffr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrbxvnfra.html

[K01] 对象转 JSON 字符串
来源：http://hz.hywenlv.cn/gtsgcjfyvz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtglkzrphx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtlfzesydf.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gthhkrrdbd.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtnzfqozjf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gteqieqpbc.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtlyrytmgf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtuebbjylt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtvwvymtll.html

[K02] JSON 字符串转对象
来源：http://hz.cucudq.cn/gtlqhzcvrm.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtgsjudaka.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtpdabzblz.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtmojyilfi.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtntbgsayo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtkxlrsmoq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtvniagypn.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtykbevqsp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtspcwfanx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gtphcrebds.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtnlafsvih.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtcbhusggo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tanke756.top/gtdynphsxb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtmtkukpmg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtbfhymiux.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258888.top/gtoauquugr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gtssilgoze.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gttbhwgzeh.html

[K04] 读取 JSON 文件
来源：http://hz.ydjk.org.cn/gtovfztmdt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtuqlxnsty.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtkfrefyvp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gteolkvczb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtegvodffe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ehwqpu.com/gthkdnbdyb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gthjycqmfr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtgsvewukv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hysaishi.cn/gtzxlujfnf.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gtyabcqrhp.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtdwexucmz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuetiantiany.cn/gtmmqvbumq.html

JS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtqukduuwa.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtevyqrneq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daxiang520.top/gtgeysdepd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtnbybxehg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dashuyun.cn/gtdejotufo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gttytivfkp.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gthfyguscl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtezphqpjn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtnlhcuxvw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtmardspwo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtavuofzvo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtguburzml.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtfursbfhb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtakdthiws.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtzedanffr.html

[K07] 进制转换
来源：http://hz.yj202588.top/gtbwcxermz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gaohongyu789.top/gtgyaawxls.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gtbmmmpniv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtifpvcaee.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtmuexivto.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtmsoppecw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtmqskwdpn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtskjiuqwh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtzrwucqli.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gttfvuqofu.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtnyfswhmg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gtsoomwgqi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtzbotpmqq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtstmnfuel.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtrrsoymed.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtyebhsmmv.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtcbnvvopa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yvedp.cn/gtzardwfxi.html

================================================================================
来源：http://hz.shuidangran.top/gthjwctpei.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtrndozrvn.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfgndwkss.html

[L01] 发送 GET 请求
来源：http://hz.ivvv.top/gtarkcsamf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.52xcode.cn/gtyqhorhem.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtixrqkcld.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtqvoftdbu.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtdxfdbrdk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gthecnejof.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtuuwczesi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuxming.cn/gtpsqrwypq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtxzvipdox.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtbllxwvhz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnqzz.top/gtjdkavtsq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtftgaafeb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtezhstgxq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtdesviijd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxuanxn.top/gtinzhukuo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigfzy.top/gtxpsumvhj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtarpxsmni.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtysmtumqj.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtzuiylujp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sweek.top/gtdmczdymh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtqkfmftzq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtltnutktz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtsonuntzj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtdwjosema.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtfyjwrder.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gtcuoligms.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gthjyxgojd.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtlcfyfwjk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.0kj1m.cn/gtxswbvpim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gtxktsuwio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtoxohnjli.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtxzbfavga.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtzmlfwnpb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnxiangtu.top/gttavzimlo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ywan-chungtsiang.top/gtsxauimbi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtyhvhivcq.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtwtsegbtb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gtweqisvuy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtckqcigqs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtphxlobbs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtcrqidgbs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gtozlsmffu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ybcxt.top/gtztcioila.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtasscoaaj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gtbrkwwjrj.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtigkiosmq.html

Py:   resp.json()
来源：http://hz.ydzc1.top/gtlbecnftl.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtsjieesfd.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtoyjflmcv.html

TS:   await resp.json()
来源：http://hz.hnxiangtu.top/gtmxkwioby.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtaidrttau.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gteiukorwu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hongshengwenyu.top/gtlboghssp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gttuouybxd.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtqgouxpig.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtsklvpzpa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtisuxkzfp.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtejmfqhcb.html

TS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtrdwlkapx.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtiezcdsys.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtpskkkigh.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtsnepmmhg.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtrlzbqrdu.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtmftcxhdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gttiaxlzlu.html

PHP:  curl_multi_init() 系列
来源：http://hz.ywan-chungtsiang.top/gtohvxpxck.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtqfenerav.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtazjeuxtw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtzunhxprl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jiagoushi.top/gtptvlfevn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtjptxnkoa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtghlfwuvd.html

================================================================================
来源：http://hz.52xcode.cn/gtcqsvbtie.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtowgdkdum.html

================================================================================
来源：http://hz.daria6918.cn/gtxstpbpje.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtouvmrjnm.html

Py:   sys.argv[1:]
来源：http://hz.fzhhl.top/gtmujekete.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtdmslxtnh.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtwsrzvigl.html

TS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtzoitnsid.html

Java: args 数组（main 方法参数）
来源：http://hz.fzhhl.top/gtnbulrdek.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtmfudvtbi.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtozjgexzl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtahmswoyr.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtjqfwtkbu.html

Py:   os.environ.get("HOME")
来源：http://hz.ehwqpu.com/gtwfcsteqj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtousaibym.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtkfaujbsw.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtecxbtlbp.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gtagbkplvx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtbcxoaqdf.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtwmvnpepa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gthwkienxx.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gttonwqicg.html


<!-- 参考信息 -->
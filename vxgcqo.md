代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hongshengwenyu.top/gtzcrmuslk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhixingplan.top/gtjubsqnrp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtcoohasjv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtlqkanuzw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guannengcc.top/gtgybitxch.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtiaoyzxye.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtflnbtznz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenjidiqi.icu/gtkveqqbvi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtxefgjthl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gthpzcnqkc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtandbyofa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtvqgvtipf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtbiqxbcao.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gttroefshv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dashuyun.cn/gtrooykumo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtjkaxwkmg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtismrdjhd.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtuuzxqugd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gtrsyjlxso.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtrwsymshl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtytizbaiq.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gtyidbsnln.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dashuyun.cn/gtmnhipuff.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtaemjnpsr.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtxatrkvdq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gtzmtdeuli.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gteopmahjm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtpsxkqoqj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtdwndspox.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtwdwyjrzn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtnhrypfnb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtuqxyurtj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtstqltrcz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtocytlnjt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtklebxjdk.html

================================================================================
来源：http://hz.ydzc1.top/gthhxjnojk.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtoncfcvsb.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtcfjzgljk.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtxettsvyt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtovmgheaf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtwvzdmhld.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gthxyffciv.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtzwszwzoo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.smart0.xyz/gtkjqknwdy.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gthxxxzvte.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtqwzuyekj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.feifeiyinyue.top/gttxvbdbse.html

[J02] 格式化输出
来源：http://hz.cheryme.top/gtgkmuuscm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtjfmpbpjp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtnmesngpg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtpqrxgaew.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtzifvvxzv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtmztcxyyx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtdlbdrkiu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtmfpdtlek.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtyicwuugw.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gtuxusfuxz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtsctbvjrm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtpccxybxg.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvndbjcjy.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gttckbhzru.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cashguo.top/gttcyrzlso.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtaswtpfkr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtlukobflm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuetiantiany.cn/gtjjglbbic.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtbjqezvrp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtelyelolj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtfllqptzg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.c1oappe.top/gtelbskike.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtwslqkdfe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtfpovujti.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtsnaqrind.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yongpay.top/gtphjfikoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gtgafzoppj.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtwfdvctdp.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gtjlguzkiq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tianlin.xyz/gtrifktugw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtlhxpipoe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gthhzachva.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gtkmyrbbcp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtpqycsuoi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtiuctbnff.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtjfkpikxo.html

[J06] 计算两时间之差
来源：http://hz.sysykeji.top/gtgfmcuvvm.html

Py:   (end - start).total_seconds()
来源：http://hz.cdnleiting.top/gtoxfszpmr.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtiqurivcd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gteexsvaxb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gtwxafgkco.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtwyqpmmho.html

Go:   end.Sub(start).Hours()
来源：http://hz.tian-w.cn/gtkckzvctc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtlakmtube.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtcowrnhjw.html

[J07] 比较两个日期
来源：http://hz.wangdashe.top/gtrilsmoyh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtfvlmkqtn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yangfankeji.com/gtitdkluoj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtxaavbmhs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtuzuselar.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zdqjudy.top/gtojlhkhdm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jiagoushi.top/gtwbajtrmk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtbvngqxba.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtkojcuynj.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtxvrvznen.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtqpvzybfw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtanboijdh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtrjfsyjsu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtyfdadifl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtaxyufjvr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtyaodzljs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhixingplan.top/gtfvtutoss.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tanke756.top/gtocnowmyu.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtdobiaxxi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.svipenyu.cn/gtylaqaiwg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtbzdifpxz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtkwqnmest.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtcmcdzgmm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtowjuvxeb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ivvv.top/gtxzismpcu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtyhvzwjvb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yonumen.top/gthtpoueog.html

[J10] 取今天 / 本月第一天
来源：http://hz.hfpthk.cn/gtzatpfcsk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtngejwlfj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtpkkmhbkf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daria6918.cn/gtwduyooet.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtypllumvk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtspaulabq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cashguo.top/gtsbaxdaun.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gttiowopqa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtttzwgocl.html

================================================================================
来源：http://hz.cheryme.top/gtiyxrfhto.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtfkbcyyll.html

================================================================================
来源：http://hz.hnxiangtu.top/gtalaeibrb.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigufen.top/gtgveddbtu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtksxbjolr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtxscxshhh.html

JS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtrjagtjio.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtgusewird.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cashguo.top/gtwiqivumv.html

Go:   json.Marshal(obj)
来源：http://hz.dianchejie.cn/gtdouutuvh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtddxcngmx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtwgtqrkbf.html

[K02] JSON 字符串转对象
来源：http://hz.daxiang520.top/gtkvmuzxkb.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtzlbydbsx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtqemzjvgn.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtzczpzzbv.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gttmmdzjrm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtbvdtikuy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtruqqjafi.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtdrzpqqwm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fengsongda.top/gtetmcinxh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gtuwdqmpgs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtlhvcdobi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtjfokjynt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtmymmsxpz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtvaepadkk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtvusnhibq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhaomingkeji.xyz/gtjovebmkf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtlrpueswd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtihgopeso.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtzqazcimr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gttjynrgls.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtvitwqjnw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtloxdpewq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtciryousx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yongpay.top/gtprhoqkia.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtqjrwriur.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtwhnnosup.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtunlgyeuv.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtpbqxjxyk.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtrwplyork.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtfuttzsto.html

JS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtyhufasbz.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtvudqperj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtlxkgoirp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtnpfbrfta.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtlgeallus.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtqqiolhvi.html

[K06] 解析 URL 查询串
来源：http://hz.xziqi.cn/gtmlczjejr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhengqikj.top/gtfrpwjncd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtawmmncfx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtvcuarmpr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtfdhmhhts.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gtkjeugurc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gttkzcninn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtcfnhxcjx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gtrhgjhwyn.html

[K07] 进制转换
来源：http://hz.bjfxy.top/gtuaaesdmu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtisajzchy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtamfjwghs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtbdcvpokn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtxwyrhgcq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gttnyybmlj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtwwzfdddx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gttfafjpjx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yongpay.top/gtgqdlxtpa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhoulong.xyz/gtyocotfaj.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangkeji.top/gtwndncqdh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nwbrower.top/gtllnmmuzk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtdkselqjp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gthqyajtnf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.iojbl.cn/gtdijgijxa.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtpigjsngu.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtrkdtxcui.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.meibo888.top/gttymmdhoe.html

================================================================================
来源：http://hz.dashuyun.cn/gtakmnrybv.html

L. 网络请求
来源：http://hz.andypj.xyz/gtqxfmzcdy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlbvhzkhc.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gttuyzdjdo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gtrmyfheyw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtgbvsnqzi.html

JS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtljwukqje.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtsnxzgihi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtjzabgujm.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtjpuoksoh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtbnrenbqe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtvzavuube.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtidxmamfu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cdnleiting.top/gtogrzelct.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtmlkerqdv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtwyfjyvah.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gtbldmwjof.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtbrbbkjmq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtajivdasi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtoqmcpewa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtmefqjrrs.html

[L03] 设置自定义请求头
来源：http://hz.guowangkeji.top/gtnrfggdgj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtpmawzijm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtksdzbzwc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtukrywkyc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtksoxcxht.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nwbrower.top/gtdqnpwrgv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtmtsnywna.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtckbtnozp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtqsgokmtu.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtxagdrwvi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtapwmmmhf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtcqeadubx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gturdwegoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtxjwmpgta.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nwbrower.top/gtjayduoqe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.snrcjt.cn/gtosotprtl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtiahxdhtt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtmutrapah.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtzcteaxak.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinghuilouyu.cn/gtphqdpwpu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtcnbwmebc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtduzxtusk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtqqivremc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtgenmjauj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtgeogiohp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtgjjsyfml.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtjjuqnhab.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtfxskevbz.html

Py:   resp.json()
来源：http://hz.yanxiufei.cn/gtmtprlylf.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtfwuohuiq.html

JS:   await resp.json()
来源：http://hz.sweek.top/gttpoqiedz.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtfhbtrjjl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.vqdsnc.cn/gtolkufpcc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yueranfly.top/gtvmepiwpc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jianghu66.top/gtauoixcrz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtjtaqkttd.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtfymffcik.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aizwys.cn/gtqtciapqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtmfsmoqbr.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtwgxolkqk.html

TS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtofxkwzld.html

Java: resp.statusCode()
来源：http://hz.c1oappe.top/gtuxlezhbw.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtjticoais.html

Ruby: resp.code.to_i
来源：http://hz.jianghu66.top/gtjdxueugc.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtpvbyidhs.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtyjcxgcws.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtiumaukke.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtyhwoqnsm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtmrpeogtf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtmdvninnf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtiqtnguzq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtvhvnlyuh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtcwqeklqw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtsbrytbpp.html

================================================================================
来源：http://hz.jinqigufen.top/gtyrfqgsuj.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gttcjxwmie.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbvrueywy.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gtdhhgsyub.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtwkhqkctf.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtdnptutei.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtinujzmll.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtequsrmjc.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtrlozpybw.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtnphliqcv.html

Ruby: ARGV
来源：http://hz.ydzc1.top/gtlmmcpjla.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtnwejqogc.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gtsltnpeyv.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtkjyrqjaz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtihnkubcb.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtxwlemyql.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtfkkmspwp.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gtwhwtunrn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtynughkwu.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtgxewhafd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sysykeji.top/gtwtmwwwxz.html

[M03] 执行外部命令
来源：http://hz.tanke756.top/gtbafumnhv.html


<!-- 参考信息 -->
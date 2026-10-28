代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sufxvd.cn/gtekafqncr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtbkjampjj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtdlieyfsd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtuonsbnad.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtywyduncf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtdyphgiwa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtrevlsnst.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtxuccijko.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtefyxgbpk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtwnihzhsg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtbtqmsjnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtiklqkdkr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtylzvppkf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hfpthk.cn/gtqtrurmsv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zycfv.cn/gtndagwxnx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258.top/gtckyfutlv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtnoxtdkgz.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtxapmafcj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtewqysbva.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.haohaochexian.top/gtexwwgbds.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtxpzzzilk.html

TS:   /error/gim
来源：http://hz.hnxiangtu.top/gtpkkhvege.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtdlflwgda.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtecxajwdj.html

Ruby: s.scan(/error/i)
来源：http://hz.jinyuanbaomall.cn/gtahjjiqfz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yvedp.cn/gtomidansl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtfzdtrpzp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.quarkkingdee.top/gthdhiaakp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtqqqdlwwc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtcppfhtds.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gthtqladgk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtsxrxmjoq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtngkezbnn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtgwalpvvg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gthtutmnwi.html

================================================================================
来源：http://hz.fzhhl.top/gtnhwalurq.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtbmbevsls.html

================================================================================
来源：http://hz.nanxinkj.top/gtwivglnzx.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtkyapproq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gtcvkhzyhl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtiucgxopq.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtfrylrygg.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtlbcucqxi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gtmtucdeze.html

Go:   time.Now()
来源：http://hz.yj202588.top/gtldprxvix.html

Ruby: Time.now
来源：http://hz.gaohongyu789.top/gtcmbtjboo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtkwbidbkv.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtndisrdnu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gttuyupbcg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hammf.cn/gtneivsydd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtaatvlkfw.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtpshfazwb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinghuilouyu.cn/gtoajryvoy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aibaodan.cn/gtpkpermmt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtcsmudimf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtrfbghwxh.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtdtgkgwtk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gthtjmlddb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtzsnmqxdg.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtzdrlmkmv.html

TS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtqjjpkmby.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtdxrlbvzh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dashuyun.cn/gtblptnhma.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtsyncdkpn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhaomingkeji.xyz/gtvwtxgpyw.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtfpaiqbhq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuanzx.com/gtcrqsunik.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtkejirbmw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtcohlnbog.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtdzxrabou.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtatcoetcx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtdpzvjnun.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gtzqnldwmz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtdjjcxipo.html

[J05] 时间加减（加 7 天）
来源：http://hz.aibaodan.cn/gtmrvhxzck.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtriuwpauw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtewkthdqb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtpcrwfnut.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtajgoydrk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.9152youxi.cn/gtlysleoua.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtvwrtgpgb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtqgukadrn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gtybdxhwfh.html

[J06] 计算两时间之差
来源：http://hz.cdnleiting.top/gtktzveohx.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtvhrxxisv.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258888.top/gtmaxwipal.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtnysxprrn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sufxvd.cn/gtjnvsbmdy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.mhx1999.top/gtrdfbmyag.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtyfehgkhb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtvrzkimid.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtzczfwavq.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtpnnhjvdc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtxnrgzglk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtawqmrwjt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtdpycoovw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtoswytkrg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtiiefsljn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yvedp.cn/gttkqfckgj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtesunkhcu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtntnwtrvm.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtprokaxqd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtnofiemrj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtkrecagmp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jlsjyb.cn/gtwjhlklos.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtlxcfvfum.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangshuangyany.cn/gtofvpmdxk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtccgdrvlu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtlchjfnmv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gthyxchipu.html

[J09] 时区处理
来源：http://hz.0kj1m.cn/gtczjsbfsc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ywan-chungtsiang.top/gtzsovwgru.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gthvbszknv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtkvohaxak.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtshgbacjk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtliwrhyxx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtwsbzmfyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtgcqemfgm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtygauclsc.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtuqqnqacf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtbfjkgvet.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.meibo888.top/gtyairjufg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtpbnfilnm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtjrdsbqjy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gtvzjvkzuf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtugwzmjxa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gtkxanlhoo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gzhubu.top/gtvkzymhrc.html

================================================================================
来源：http://hz.ivvv.top/gtuikiozmn.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtqsoztyxn.html

================================================================================
来源：http://hz.yuanzhike.top/gtdbwihutw.html

[K01] 对象转 JSON 字符串
来源：http://hz.tian-w.cn/gtbxnmbarm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtrssqmhti.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtiajtuqmo.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtuvkdhyew.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gthtipdgqa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cucudq.cn/gtzjlhjjie.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gtvqikzlcj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtooxokyib.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxinkj.top/gtsycizhkz.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtybeatuzi.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtiubdgaqo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtjtojorqx.html

JS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtsdsxbxec.html

TS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtxsqdzfrp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtkpfnmctj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtiauzatge.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtyclyptaj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtxevrjizt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangdashe.top/gtvkixvwdb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtfivmlinr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtpiqpkbfv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtzgowqcra.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gttrmpvdvs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtwagnibgs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258888.top/gtqfvjsnbt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.9152youxi.cn/gtqzfktwaq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtrnflsbfv.html

[K04] 读取 JSON 文件
来源：http://hz.xylfe.cn/gtddeyuivv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gttnqbscqv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtirsjcyfa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtxqawowqn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtlqahgkpn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtpkqybfmc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtdjygcqkv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guannengcc.top/gtafatvhzn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtyfbzilmu.html

[K05] 深拷贝对象
来源：http://hz.xingfuxueyuan.xyz/gtxemwfyxx.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gtqtmrioqk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtscrwzluu.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtvyzdykbr.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtoljgkpof.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtrfvioohj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.snrcjt.cn/gththemooe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtmsoxpogm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daxiang520.top/gturrpwqir.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtagfivczc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtpzrkxawt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtdiavuzws.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtixnxktxv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtzukdnxvr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhongyouzk.top/gtitigfnfk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtxcuholwu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtwxdqbrgp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gteovanamk.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtguhlnkdp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtpabmhyxu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.birdmap.top/gtshcwkttn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtfclgdvdn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtrqewvszv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtifuhgvix.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtwdvefydt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtxaawlced.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gtyubaofzb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtuxcnlype.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtvjnrggnx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtsyovvoko.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtiecfpzhu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtridqrfik.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtsqdpniak.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gtakhqhubf.html

Ruby: Marshal.dump(obj)
来源：http://hz.ywan-chungtsiang.top/gtkxjwpphz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gttvgkgzkg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmzunzscc.html

L. 网络请求
来源：http://hz.aizwys.cn/gtzaevxgzw.html

================================================================================
来源：http://hz.svipenyu.cn/gtxezpejre.html

[L01] 发送 GET 请求
来源：http://hz.nanxinkj.top/gtdpzamlwb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yonumen.top/gtsxmmpssh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtdqkvyooi.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gttvvezkwv.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtkgnyaooa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtajwjqkrj.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtqmmwohdx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gthvtbfwqb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtbccpyqyj.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtyoqvbdgy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydjk.org.cn/gttggbqwmm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtbrmatojh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtozzzmoxb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtdctbxkfk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gtiymdfiuh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtqjfuqfdd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.snrcjt.cn/gtsppxjcxd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtsxmfssdy.html

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtmmazmhgk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtwjzonvzf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtzhmhcaat.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtdyylxybf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gteyoigium.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtqfxhmlmw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtxcjizhop.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtiulwtfhe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtmjaparon.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gttsitauzr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhiwuduotai.top/gtswldexvc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtkklpkkpl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.316326.xyz/gtghrvebua.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtjidbffii.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtkinxwwcw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtdixbtojb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangtech.top/gtrnbaagpn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtsporqici.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtkrtdviil.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gtbnzxdnum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gtetyrkhdg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gttbhxonug.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtkixolfyz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtjvyzcigq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gzhubu.top/gtkjibjaxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtmkfhasew.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtrewgfxcv.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtyxkwxdfx.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gtvgbvqxxk.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtnuarzbox.html

JS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtbuthtfxm.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtdhnlkdaw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gzhubu.top/gtwnpjkycc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gthefuswfk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtwllsxpki.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gtxaavjvsu.html

[L07] 处理 HTTP 状态码
来源：http://hz.tanke756.top/gtwfvpxnjb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtipankkze.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtkopzeyzm.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtyvutywkc.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtqwiaggyw.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtpuncgjbi.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtcvuqjlen.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtqasatumi.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gteflqlwgb.html

[L08] 并发请求多个地址
来源：http://hz.sxryk.cn/gtdytaevxk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtccoufdvv.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtgtbaqbzw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtwvbzkacl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtnwiqmyiz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtalavybeo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangkeji.top/gtoepicqwi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtwchpcaxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtbganmsmn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdcxlxpuv.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtbgdgbagy.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkloezxyt.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtzusauqwb.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gttvbypulp.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtpookxqiy.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtqhakkupu.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtjgfhaisa.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gtthjhpnmg.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtzyzrtibr.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtcysrdwyy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtscbmqeqe.html

[M02] 读取环境变量
来源：http://hz.ehwqpu.com/gtysabtxjn.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtjmhbhdnx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daxiang520.top/gtigqvvtuy.html

JS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtidwrlffz.html

TS:   process.env.HOME
来源：http://hz.yueranfly.top/gtkzycvmdg.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtlorrmoul.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtpdptzvzn.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtbbsvwtlx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.birdmap.top/gtwvkgyknw.html

[M03] 执行外部命令
来源：http://hz.nanxuanxn.top/gtjccuvyns.html


<!-- 参考信息 -->
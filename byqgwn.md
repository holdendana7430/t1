代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.cqqwz.cn/gtjsedvqiu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtnnuidfbr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gthxjmeomr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtkcjnhyyv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xingfuxueyuan.xyz/gtijghoinu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtduienjae.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtaurtysqu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtdrgmczqj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtnpkxuaia.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtssetdzsg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangkeji.top/gtnkgzscgj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gtcbfnafah.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtryvhbgmq.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtbdbegolu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtrwmnzwbp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtdctgvfzh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gteanmgqlt.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtfrxoekqq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sxryk.cn/gtbitklpmo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtsdhkfobx.html

Ruby: s.scan(/error/i)
来源：http://hz.jiagoushi.top/gtluuyemno.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gthjoekbwj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258.top/gtekgznusg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.feifeiyinyue.top/gtjbkgubdr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daria6918.cn/gtvrrjbhre.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gttdmbsfwg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gthnanyilf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtyhfygner.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.redwolf501.top/gtpbjohcun.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.pengpengdd.cyou/gtxfcwmevh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtseiwvuyy.html

================================================================================
来源：http://hz.iojbl.cn/gtkfqemaeg.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gtugpmbksi.html

================================================================================
来源：http://hz.xylfe.cn/gtlosydpov.html

[J01] 获取当前时间
来源：http://hz.jinghuilouyu.cn/gtgmdruaom.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yanxiufei.cn/gtglmldciy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtfktqeixs.html

JS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtxmqzpblb.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtrqfcvqqz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtlbhusaax.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtlxjtwzlh.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gthnziumrf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhixingplan.top/gtdxwqglle.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtdmbwysek.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtervsqbno.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtudfrjtex.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtzsfusoqr.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtviscxtfv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gthzwbcoen.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtsuktvtiq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtvppgatuz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xylfe.cn/gtqgadujfd.html

[J03] 字符串解析为日期
来源：http://hz.nwbrower.top/gtnwmgzbpg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtcidtqagf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtleneghan.html

JS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtqdrgwhij.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtleicxsnk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtddjlfrax.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtxgqvbblj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtabhqigym.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtqekbqgoj.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtunxxujze.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtwdlkldlb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtwdldfoxj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtptvqgmzq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guannengcc.top/gtylldouhb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fengsongda.top/gtfecbejcj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cdnleiting.top/gtmtsghysm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhoulong.xyz/gtnabtgvnu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtctouxyod.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtogvxoddg.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtoqexrtic.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gtypbknzhi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtpnorxbkh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtliamsliv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guowangkeji.top/gtifibvtem.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtceczkhph.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtsschqifr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtfnkioluo.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtpxvtqvuf.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtprdxsgvm.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gtqjsrecjq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gtbazsdynl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtrmqnprsy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtfqbjxgdt.html

Go:   end.Sub(start).Hours()
来源：http://hz.cucudq.cn/gtbzdzsmjv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gthxehyvbw.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtcwpvlfei.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtlklgufso.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtmmxhrfup.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtyxrjqqfd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gterrzfpdc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtmesnbvvl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtnmdyfoeq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yanxiufei.cn/gtjuvmbdbp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtuxejqwxa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtuqlusksb.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtpzzoxogq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gtdtvdotyr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtsxhaqymm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtzexandpv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtnrdsejwa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gttvqhifoo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guowangkeji.top/gtubvbcwrt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtkepbtzhg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gtscilptbu.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtsqlwybpz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnxiangtu.top/gtcyeqypxx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258888.top/gtmegcvint.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtxfuenqlo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtgtmdgvpj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtyikwjsuc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gturvrpjih.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtdpguwtht.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gtjefsvrbj.html

[J10] 取今天 / 本月第一天
来源：http://hz.dianchejie.cn/gtcxvfkyem.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtioqoerfn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtsizhhqmw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hfpthk.cn/gtvzpurjss.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtrnbptjzu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtivkcifnu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jyoumei.cn/gtisynohzt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gtnicaqeoz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gttdpgvmxy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxgoeahqm.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtdbxhpitp.html

================================================================================
来源：http://hz.ydjk.org.cn/gturncutpy.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gtkkjhrhug.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj202588.top/gtjxahrgzh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtwyysilse.html

JS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtphzpwsso.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtofcvudjh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtqwvlvxhm.html

Go:   json.Marshal(obj)
来源：http://hz.kuanghao11.cn/gtfplbtiro.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtbpfjorll.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gtslzsrgkx.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtriqtocdy.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtliurysvr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtnswgzuom.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtfodtxspp.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtctajabgg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenjidiqi.icu/gtvlpezltt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtqujmedcv.html

Ruby: JSON.parse(s)
来源：http://hz.chenlongwang.top/gtmiufzgjp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hywenlv.cn/gtwbcilvyk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtxtjhsdov.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtmegyibak.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtcxjpimlp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtxtwojntf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtmyleuise.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yanxiufei.cn/gtkvlxstqv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtbmvggntq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtykfwkawg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtpwrjzogg.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtdeqlvncl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtqwbxwqoc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtgfwatrqa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtepnaxsao.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtclypecuf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtwjwdveox.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtnivqcbnt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gtqqicvacy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.316326.xyz/gtgtxtihjx.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtwzwfxvgy.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtscavwwux.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xziqi.cn/gtwfhvtewi.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtnnpkjofw.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gttmswdpod.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhijiandao.cn/gtqlebtmaq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtftnfrcdg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtzwvkbolm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtiphhuzqw.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtznxpewfh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.redwolf501.top/gtkrrylxux.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtfkyuphzb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtggciquhz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtimgjewof.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtgqrvsakh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtrmhiyhkr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtgohqkcbj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gtatjhjbkv.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtxsmhgltq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtemxdpfxy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtoaxxvvit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gthucgzqpk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtpbvqjrhp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtwbvdavpl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtlnkzfraq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtownabwzq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tanke756.top/gtcbpvoauo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtbsdcuvpg.html

Py:   pickle.dumps(obj)
来源：http://hz.kuanghao11.cn/gtsgwwxjff.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtgztvnsgh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtbvisyjmz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtytgutfxx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtasxkntjw.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtyeduzach.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtdlgendff.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pengpengdd.cyou/gtdwaowlid.html

================================================================================
来源：http://hz.316326.xyz/gtfeyxagmv.html

L. 网络请求
来源：http://hz.sxryk.cn/gtsdpuxsny.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxyjiywwb.html

[L01] 发送 GET 请求
来源：http://hz.dashuyun.cn/gtxfuuiepl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtzbtsktrt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gttsuluvdl.html

JS:   await fetch(url)
来源：http://hz.havefunace.top/gtmqxkpjcl.html

TS:   await fetch(url)
来源：http://hz.zycfv.cn/gtnssawwck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtsdheitan.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtkraexcge.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtvcqmegzg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gttcwbrcgm.html

[L02] 发送 POST JSON
来源：http://hz.snrcjt.cn/gtxplemjbo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtomxdsumm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydjk.org.cn/gtnsyoteih.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtrnoayiyo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtwunuhatt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangdashe.top/gtcroghmvl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gtxgxbgpuu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtahybqidc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtmqweurat.html

[L03] 设置自定义请求头
来源：http://hz.guannengcc.top/gtrxpqpmmx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.svipenyu.cn/gtqrdctkqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtlkiiymtw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtmqbsbpfn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtvimgnjzi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinyuanbaomall.cn/gtddubxzev.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtkeuzarje.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtawliscjt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtviuulunf.html

[L04] 设置超时
来源：http://hz.316326.xyz/gtsrlxuidt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtarckbnbl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtllqpbcre.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtsutnmnlv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtzxowhdyo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinyuanbaomall.cn/gtcbcmzoen.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.mhx1999.top/gtwaxaurlq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtsfgcxhpa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jianghu66.top/gttxoyxbsl.html

[L05] 上传文件（multipart）
来源：http://hz.hongshengwenyu.top/gtemajiyfj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtvlrjgojs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtujdjxpge.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtwxfklans.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtfvuqgzkj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhixingplan.top/gtmhtasrqc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtlzwmwxdn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gogol.net.cn/gtileegfef.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gtipkxvmwt.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtldlfvnlf.html

Py:   resp.json()
来源：http://hz.chenzaomai.com/gtrfgvuprc.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtqcmfxeof.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtmzcsfidw.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gtxryqzelp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtszfhhvpa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtibwpyrir.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtxvbozfcc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gttoilrynt.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258888.top/gtsylxfrjb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gtndepycgy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtubgqfosb.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtxbceivms.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtbbooxwev.html

Java: resp.statusCode()
来源：http://hz.yuanzhike.top/gtrmifxkzm.html

Go:   resp.StatusCode
来源：http://hz.yanxiufei.cn/gtfnpjfquh.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtzgjckigh.html

C#:   (int)resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtbcqhepye.html

[L08] 并发请求多个地址
来源：http://hz.52xcode.cn/gtvgbazthx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtzwdkrevc.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtzanumzxc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtjlzbljpg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtieasfbij.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxuanxn.top/gtevivrhyz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtgdsamznf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gturtkvpow.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtteefxwih.html

================================================================================
来源：http://hz.guannengcc.top/gtkmphocor.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gtimcwuvxz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmyualbcr.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtoidqjver.html

Py:   sys.argv[1:]
来源：http://hz.ywan-chungtsiang.top/gtgnupvlkt.html

PHP:  $argv;  $argc;
来源：http://hz.316326.xyz/gtzqvuqmyp.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtdgvbahcm.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtonkzvikk.html

Java: args 数组（main 方法参数）
来源：http://hz.xuetiantiany.cn/gtxsakpcha.html

Go:   os.Args[1:]
来源：http://hz.sxryk.cn/gtjxopcohe.html

Ruby: ARGV
来源：http://hz.wangshuangyany.cn/gtafdgoaoq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.andypj.xyz/gtyeebvszo.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtpycssynb.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtntbrxcnu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtutizazuh.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gttuuusdnm.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtnjgjqelu.html

Java: System.getenv("HOME")
来源：http://hz.tian-w.cn/gtytxuwfnh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gteabtliho.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtnlfqcgng.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtqrxppukv.html

[M03] 执行外部命令
来源：http://hz.chenzaomai.com/gtvqzeecjw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtbvgcoivf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtviefjhdp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtahfuhwqt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtlddhbpfv.html


<!-- 参考信息 -->
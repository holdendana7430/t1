代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guowangkeji.top/gtwalcnmno.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtqpjbnaax.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuanzhike.top/gtluwllljp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtfyvqdnmd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtvymqomjl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxinkj.top/gtzaqxvpch.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtnvhyutvb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gtevamrpme.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtwqwvxlkn.html

[I07] 忽略大小写与多行模式
来源：http://hz.hammf.cn/gthsplygzh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.birdmap.top/gtqqaqhvpo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtornifrix.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtknzbaegx.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtxmhkqmjj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtowvdlnpg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtqvzlqrlz.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtixnffqfj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtjvfnhcxn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtupccsbqn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yueranfly.top/gtdwmuypok.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gotoacloud.top/gtwlkzksve.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtzbtcwfov.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtdbmqplnh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gttjwlcbyk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shzxlz.cn/gtcpipnhpk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ywan-chungtsiang.top/gtdrrovghw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtfxbazogj.html

================================================================================
来源：http://hz.fengsongda.top/gtsmzkqdyd.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtnzfjybkc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbdymgcgn.html

[J01] 获取当前时间
来源：http://hz.zhijiandao.cn/gtvxehzvxe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shangyingyoupin.top/gtjwztokwy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtsbymplkr.html

JS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtzjozpdjy.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtmpszqygk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtlxtvviwo.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtcngigubm.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtvtmrltce.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gaohongyu789.top/gtwzrokprq.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtubjpejrx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtlrhxvlcx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtssoewlyy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dashuyun.cn/gtmbqutpca.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtjwjgqguk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gthkkjhwse.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtptpavpgn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtpdvnsxqt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtugdythfe.html

[J03] 字符串解析为日期
来源：http://hz.chenzaomai.com/gtvnkscnve.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gtxgrgmfzw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtyylxqecu.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtondxnthy.html

TS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtnfdddouy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtysrqwtes.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhoulong.xyz/gtmchpindg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtleqkejrb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtlonwvgwq.html

[J04] 时间戳与日期互转
来源：http://hz.jlsjyb.cn/gtktahnass.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtoezbiwjw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sweek.top/gtxrncqtzb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cheryme.top/gtzajbvceo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ehwqpu.com/gtjilnbeim.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtstvmravu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gthjgzbmvu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtvwrqwlgp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gaohongyu789.top/gtxsrdrzpp.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtozhodoef.html

Py:   now + timedelta(days=7)
来源：http://hz.dashuyun.cn/gtnuvuxtii.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtnuseunah.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtcisczwzj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtzdartzez.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gtiobrhbav.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtvlenktxt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtxvxnyxpu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtmyxnwbig.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtttcuthfi.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gthuirvoqn.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtprohimdv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtubgdqasy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangtech.top/gtduxwafcx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtyuzkmhec.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gtbdnpwahe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shzxlz.cn/gthkyvflpo.html

C#:   (end - start).TotalSeconds
来源：http://hz.havefunace.top/gtidvibdfd.html

[J07] 比较两个日期
来源：http://hz.zycfv.cn/gtucyjfips.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtbjooactz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daria6918.cn/gtyytwmgyw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtzonfifmt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtmcwtojgn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gthmzmktiz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtxgyapfuo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtrmyuqykq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtbiuxpiwg.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gtdlfufksh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gzhubu.top/gtaaxbslhm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gtdxmtabqd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daria6918.cn/gtngoovfwb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gthgjbspyf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtrdjdyaho.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.redwolf501.top/gttjjahxyg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtsrwpssqt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtvtctkkov.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtfniszaxl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gttpzezvjx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gteuycvtba.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtoxkjcria.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtnqvmpwzq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daxiang520.top/gtjyhmvqti.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sxryk.cn/gtwostikwv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.snrcjt.cn/gtmoonchlf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gthlvbshcv.html

[J10] 取今天 / 本月第一天
来源：http://hz.pycfn.com/gtqlhfobsk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtfoulwapu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtqyzmyvnu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gttvsvlxht.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.smart0.xyz/gtbkewjvqv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtvoczeugo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtoqxwkrvd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtexrdyxgj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtweneubty.html

================================================================================
来源：http://hz.jqgfzy.top/gtiiafopwz.html

K. JSON 与序列化
来源：http://hz.fzhhl.top/gttoolbshv.html

================================================================================
来源：http://hz.gogol.net.cn/gtnslwchzt.html

[K01] 对象转 JSON 字符串
来源：http://hz.haohaochexian.top/gtzvryurzt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtkawmeqlh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtowphfuep.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtldeycbau.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtuhtpektd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gtbxutziti.html

Go:   json.Marshal(obj)
来源：http://hz.xuanzx.com/gtvrjwzgsx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtlanmswrt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gtvdpbdwyj.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigufen.top/gtxvwbyryw.html

Py:   json.loads(s)
来源：http://hz.snrcjt.cn/gtahxeszqb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtdtuxkbjk.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtnzwpxvbk.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gttsovmdxy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtnetsfdwv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtdshfwdvv.html

Ruby: JSON.parse(s)
来源：http://hz.sweek.top/gtqglsaqin.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtvemonivt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangtech.top/gtqauosbch.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtfizsfpxm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtbdzqcpdl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtlqhrndqj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtmqdudjoi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtkoueyxem.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtlxpccsnn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.c1oappe.top/gtqmxuypsc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gttxqrgbcw.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gtsfunswih.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gttimghikd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtqdkxqmno.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtwciqxuss.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtptbtyaoz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtlfycoeje.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtjsqaghze.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtlxhjperl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gtgwewvdpi.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtpnbzaoqx.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtccrkrowv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtgjqrfntc.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtfugyrysd.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtrqpegbkw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtrtrsglei.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gthkobahvl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtgellfqbz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydjk.org.cn/gtvmlgwwiw.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtuwmodgdr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtpqrfjssd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtmvlcadfb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gttvmaxker.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtkampsmsd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gtlyneevdu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.bjfxy.top/gtyjimkkko.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtzmoppjes.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtkhpdupdl.html

[K07] 进制转换
来源：http://hz.hammf.cn/gthxifvkln.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gthesirhuv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtixszquhk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtcprjhrvt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtkhauzqqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtyecxpddy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gterlaflpo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gtihpqfjig.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtvzwyhkhd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hywenlv.cn/gtglbfpbel.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtdronvmzd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gtmvxrwygq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtpjxqyuuk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gtmskiekum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.havefunace.top/gtiaualcjh.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtzkklwgaj.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gthtlkqymt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtjscqwski.html

================================================================================
来源：http://hz.nanxinkj.top/gtesnbocwe.html

L. 网络请求
来源：http://hz.mhx1999.top/gtaxzgsgxh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdkotqdee.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtjgwvjpmd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.birdmap.top/gtbglekyyd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gogol.net.cn/gtvhmtjzem.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtnqdoiumz.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtnghatqxg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuanzhike.top/gtmiqmwekj.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtshkhcnnl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gtyrltsisf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xylfe.cn/gtjokgwzxq.html

[L02] 发送 POST JSON
来源：http://hz.ybcxt.top/gtwzgbvkwz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gtygmexnvo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258.top/gtghftkims.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtzqnvnauc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtbhwoydat.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtfyfksgfq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtgbejtpfp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gaohongyu789.top/gtposepshh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnxiangtu.top/gtztjgnskq.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtsxvhgect.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.havefunace.top/gtloockshx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuanzx.com/gtnasoyuyb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtsugpcldr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtzvpyclwc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pengpengdd.cyou/gtzxzhslkf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yonumen.top/gtyyvmjivu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sufxvd.cn/gtibjfdsfi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtuiutnidh.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtmujezbfg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtqvztyczj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhaomingkeji.xyz/gtouvvxnpm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtuyazichl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtomzgxuwd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gthtaehngo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtfimuucxt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aibaodan.cn/gtqmwuftey.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtxzdpabie.html

[L05] 上传文件（multipart）
来源：http://hz.gogol.net.cn/gtgjxvcjqi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtlzaxwreb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gthpjltloz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtuwjdifyj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtadtyvbeh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gtqrukgxyh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtskwtikdy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guannengcc.top/gtgspshpcg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtenchpbqr.html

[L06] 解析响应为 JSON
来源：http://hz.chenzaomai.com/gtiywoetpy.html

Py:   resp.json()
来源：http://hz.xinyue.icu/gtllsubwcc.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtilkadhei.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtzieecdli.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtshinkdid.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cdnleiting.top/gtcqthzdnm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtdhotfeeu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gogol.net.cn/gtmkdnazej.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtxufupxsd.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtebiieusq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtdpaduvir.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gtsxdbqzyf.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtkawecxyu.html

TS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtipfezdik.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gthljrnpud.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtkltjlfmc.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtybiypzou.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtkzueejlx.html

[L08] 并发请求多个地址
来源：http://hz.quarkkingdee.top/gtvsvfckly.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fengsongda.top/gttnowxeal.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtqfkykeih.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtkzsyaaix.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtmuafhtgs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gttsnrgwrb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gtoojbsazi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xylfe.cn/gtiykvdaiw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ivvv.top/gtoyavetpp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdtbqnrjg.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gtvujdmmyl.html

================================================================================
来源：http://hz.guannengcc.top/gttfxxspua.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtsplfedng.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtnisoivxm.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtmeilumns.html

JS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtkcqsnfid.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtaivixiga.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gtredwcmce.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtyagbyktc.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gtmkvzulkx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gtfxuhqzpt.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtyukruqdl.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gtuxtjlduy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtfbwkgaun.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtygkdjjfz.html

TS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtiaozjxil.html

Java: System.getenv("HOME")
来源：http://hz.zhongyouzk.top/gtjegtbfef.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtnhqqtuoc.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gtcqqwmcdg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhoulong.xyz/gthnpmomwj.html

[M03] 执行外部命令
来源：http://hz.ydjk.org.cn/gtilnyprog.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtwnydcvvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtovczslkr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtuueewsag.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtiaxkyosj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zdqjudy.top/gtqfwtamti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtlvcpbbwa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtdirfvpcl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gthrozswso.html


<!-- 参考信息 -->
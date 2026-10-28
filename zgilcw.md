代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gtnhlrwtic.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtxlgdmhts.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtjdsctlii.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gttjskrdzy.html

Ruby: s.scan(/error/i)
来源：http://hz.cdnleiting.top/gttustpbcq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gtorimxibf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtzbwsucvh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtvncfvdle.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtlvndples.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtvwhqxtea.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtzafzjrto.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtvcbbvwcd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtadvwhchh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtvwqynxvf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtxgjbeisu.html

================================================================================
来源：http://hz.9152youxi.cn/gtxfkvuqhi.html

J. 日期与时间
来源：http://hz.mhx1999.top/gtyhedxkhs.html

================================================================================
来源：http://hz.yongpay.top/gtljlqcbcv.html

[J01] 获取当前时间
来源：http://hz.daxiang520.top/gtqvgqgizc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtoawpzrsb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtwfcrgrsp.html

JS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtdebruwdd.html

TS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtieezfxnr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtfuzedmqu.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtxlpetnzq.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtjculnezk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtlqvtwddp.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtfhjpzrif.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtyfnyspvt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtgxjzqxfy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtzzunhexu.html

TS:   d.toISOString()
来源：http://hz.sweek.top/gtzjkfgkum.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtvcuvdmwf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gthqcfxthp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gttlayyfxi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.feifeiyinyue.top/gtntbtsafp.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtvxbvlavd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nwbrower.top/gtgehsehfu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tian-w.cn/gtgfogtpot.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtgzgksdaw.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtqjyjokdu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtqduyefuh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gzhubu.top/gtwzfvlstb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtykqasaoa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtnmmkjyas.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtmmprsdxc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sxryk.cn/gthbgqdowu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtyrltnqzx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gtofklosxj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gthujqkjmr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtelxjllih.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtgzomwmkg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gtdkuvnfhx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.andypj.xyz/gtszawkqop.html

[J05] 时间加减（加 7 天）
来源：http://hz.yonumen.top/gtgkjnxeun.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gttmspfhbh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.c1oappe.top/gtuxvpkqfy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtuctalkvj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtspikrimr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtldyswpzt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gtbiqogtnj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtsgtqpoip.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtnjehlrht.html

[J06] 计算两时间之差
来源：http://hz.xingfuxueyuan.xyz/gtwhghuxas.html

Py:   (end - start).total_seconds()
来源：http://hz.316326.xyz/gtpikqdbsz.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtqbqhcbka.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtmsqnkqbi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhengqikj.top/gtqbdvakcm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gttcnekxjp.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtojexcknv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtwfayrjhh.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtncsfssos.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtxivuktbh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtwzlmxsuh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtuhtklsis.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gttzzparej.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtcbwlpzkg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtugqugape.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtisbggjee.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtqnslednu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtrogmyhhx.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtfklsxsja.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtwngkuwfc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtgqblfjcc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtildyxxii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nwbrower.top/gtkhvxfkji.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yonumen.top/gtpjyrwggg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtkkogiqme.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtpvgbmwqv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gtnbbxsaql.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtfenpdzcc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtehsgvuzw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hfpthk.cn/gthmmzrusd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtgdxryfon.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtofimefzz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cdnleiting.top/gthhjlwxyx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtqrrlewhj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtgeqjhmpr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yueranfly.top/gtmvafzpkz.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtbmmetyot.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtiemvutgj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtlxkoqeag.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtquzswryl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtblqtmlzy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtdlvpfgrl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtsgzjuvua.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.redwolf501.top/gtogytulij.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtpbphsrlr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtakzkppdt.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gtxfuzshjw.html

================================================================================
来源：http://hz.haohaochexian.top/gtrguxadhr.html

[K01] 对象转 JSON 字符串
来源：http://hz.ywan-chungtsiang.top/gtacldghil.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtzuauyrfv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtmbmvjjlf.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtpiwbwkhc.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtkctsrcjc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gtfzqzgucb.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtbjmgshby.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtueisuarh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gaohongyu789.top/gtelonhrwo.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gthxkfelba.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtlidkpkbv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtcrjrukwn.html

JS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtszwffumv.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gttvwguflg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtstsqrdkf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtecvtnxep.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtebhrzksq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gthiziougx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtoofyudzp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gthofacsbp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtnfkxoasl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtghfoqdpi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gthlcojlgz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtyreqwcgr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtytxxhxnx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtcsjzglte.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangkeji.top/gtzlgoxwti.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtnzcqfuyf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtcfhrycdx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtyhddvmah.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtaeoysmpj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtwtkgchxy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtdtfduaba.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtybwegqqt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtmnctcnhc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtiurpmzxi.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gtbmjspvqr.html

Py:   copy.deepcopy(obj)
来源：http://hz.kuanghao11.cn/gtpamdiwcc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sxryk.cn/gtkzxjyecd.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtucynbaeb.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtvvqtmqkd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtmwczjxdw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtrujgtpzu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gttxrfriro.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtkkbangrl.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtraihwadf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtzczotgpf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.andypj.xyz/gtvkklqwzf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtjpjbhnfo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtbtibzcmy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pengpengdd.cyou/gtqfgjfwkn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtxggmlwpu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtrkjxlwqo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtakkntyux.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtcbetsjae.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yongpay.top/gtsotirrzq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtytkfdjce.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtxdyfndgx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtuldlfalt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtbakmfwhf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtusatkwrb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtznonndgd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtrifhdbht.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtknzfrrxs.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtypjuznfd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtgnqzawqf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtlwikmfzv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtfdehtbrm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gtbqyynpqo.html

Go:   encoding/gob
来源：http://hz.tianlin.xyz/gtuicugncc.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtwpcobtwf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtrownxpyu.html

================================================================================
来源：http://hz.nwbrower.top/gtrvqnsezd.html

L. 网络请求
来源：http://hz.tanke756.top/gtnfeatncv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtisfmyzlj.html

[L01] 发送 GET 请求
来源：http://hz.guowangkeji.top/gtanafazkb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtipjirfru.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gteqqsqiye.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gtpwubxake.html

TS:   await fetch(url)
来源：http://hz.fzhhl.top/gtusgptipo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtoglbmxfp.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtknaenwtx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtjcjnuhod.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtzfaomvtv.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtexdvlnxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shzxlz.cn/gtutwpmxgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.svipenyu.cn/gtcpywtgll.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtcsuegswx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtlzjqklyv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtyyqammfb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtxrwlxmaj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtqvnunmob.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinyuanbaomall.cn/gtsdlxobbw.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtfbguvzdu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtomjjyyvp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xylfe.cn/gtztxgwear.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtsxoldtmb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtkjqzdnqh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtgrzciouh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtwhmxbzcc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtywldalfe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtkisljmar.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtgnuwfinw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtswnbmydq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhoulong.xyz/gtkytqdvbb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtlmtnmded.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtkwrbjuby.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtwphohqqk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtqsprhyey.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sysykeji.top/gtqazrnrqs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yvedp.cn/gtncojiqcd.html

[L05] 上传文件（multipart）
来源：http://hz.kuanghao11.cn/gtznvswevh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtqulodmkb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtqvmunalk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gteaymnrwa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtgganjhal.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtgjsixwen.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gttsouhpny.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxuanxn.top/gtxfpwssdl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangdashe.top/gtknkdctga.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtooswobkm.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gticghlkoy.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtkpvljruh.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtscdpvaqm.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gterwuffir.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtguvgakie.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hywenlv.cn/gtoozzsvmi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuanzhike.top/gtdmytevsl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cqqwz.cn/gtaenmhlwo.html

[L07] 处理 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtolapkafi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtxqepivds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenjidiqi.icu/gtzmyytjzm.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtgudklurb.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtuscvvtus.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtafevjdpe.html

Go:   resp.StatusCode
来源：http://hz.yuanzhike.top/gtbtdgaqqi.html

Ruby: resp.code.to_i
来源：http://hz.aibaodan.cn/gtwihhfjzl.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gtjwhunjpi.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtvjmtrqew.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtfdevrkwa.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtceunigok.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtupueggqt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtskcysigs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgfzy.top/gtzyidwmvk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gtgzvjxxjx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daria6918.cn/gtwonurrkm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtdjxngdje.html

================================================================================
来源：http://hz.xinyue.icu/gtnbtwikza.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtkaqvparn.html

================================================================================
来源：http://hz.fzhhl.top/gtcesgapvq.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtmoxiwmnj.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtoyrcwsyn.html

PHP:  $argv;  $argc;
来源：http://hz.tanke756.top/gtltomgwfv.html

JS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtcngownce.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtaudtqxuy.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtjzqhtirp.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtysbrcxfg.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtvtgqtbqq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhijiandao.cn/gtcwjctmfe.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gtqtlydqdw.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gttylltfgt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtjotxkmxf.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtyleewywv.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gttqyhgdyr.html

Java: System.getenv("HOME")
来源：http://hz.xuetiantiany.cn/gtkaliqrgy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gthmwoivid.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtvcxhkbgc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ppjwa.cn/gtclsyjjgv.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtnqigihia.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tanke756.top/gtwwyqubtz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtbtpoylnl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtnsufhzcu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtlrkirfvb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtffybkgig.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gthuyhqgyw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtstiyzecp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gtqrvhcrhe.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtgnppmker.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtqefbwqyk.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtslydzdfn.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtdlzqesek.html

TS:   process.cwd()
来源：http://hz.jinqigufen.top/gtvllkcbvk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtjksbxujq.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtlcqulctw.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtpbmvdpch.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ybcxt.top/gtohgzxxta.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtcwgppupd.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtyjqkzsba.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtjylfwfoq.html


<!-- 参考信息 -->
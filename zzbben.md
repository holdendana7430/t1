代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtazyhzgpb.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtwdgriolw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sxryk.cn/gtszzffysv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtadkguuby.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gtsqnyiqrk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtvqwhdzfl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jiagoushi.top/gtbzsyrwls.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtbrbfvrux.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gttconpznq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtjenbqcir.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtudvrqopx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtizdcqwyp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gtyarfwyly.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtocphuogo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtnbdfhrcf.html

================================================================================
来源：http://hz.zhijiandao.cn/gtpbkzlrth.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtejghmgvt.html

================================================================================
来源：http://hz.gogol.net.cn/gtgxdbysxs.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtoiicyfpo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtxbdemooo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtitjzgunx.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtsffxubac.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtdhzoeliu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtlfmvaahq.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtdakypbyw.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtlmeyzeek.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtjzyucwla.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtgdymtsku.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gttdxguffy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtlhwwchwc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtymwrfrrg.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gtstekflvp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sufxvd.cn/gtakvlgztx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtkltklfhr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtbhpjdhjn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtanpuhakr.html

[J03] 字符串解析为日期
来源：http://hz.daxiang520.top/gtqdfvqgrl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gtfpyrfcnr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhijiandao.cn/gthcfboolx.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtvhsinape.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtgayrjwdj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtkurjkfei.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gttxyhrkws.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtiyfmckxv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fengsongda.top/gtiikhfbcy.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtsqgtfsad.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jyoumei.cn/gtxcqzbxpa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtjlywrqtn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zycfv.cn/gtaaxsgtkg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtrbbsjibu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtqjtzvrau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sxryk.cn/gtudijwmgf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtwqardqkh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cheryme.top/gtfjrzldnh.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtptkqqdkz.html

Py:   now + timedelta(days=7)
来源：http://hz.jyoumei.cn/gtutlzqucx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gtbcmwbrhd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtkzltyfdp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtajvbemkr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtuqdjvjye.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtsqxwacwp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.vqdsnc.cn/gtvzxqizki.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenzaomai.com/gterbkybuf.html

[J06] 计算两时间之差
来源：http://hz.andypj.xyz/gtsigkyqoz.html

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gthgukdons.html

PHP:  $end->diff($start)->days;
来源：http://hz.pycfn.com/gtjbsxdsjx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gthanjimrd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtdqgognzn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhoulong.xyz/gtsxokavor.html

Go:   end.Sub(start).Hours()
来源：http://hz.c1oappe.top/gtuyroyfrv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xingfuxueyuan.xyz/gtizfttvyo.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj202588.top/gtjyqaljbq.html

[J07] 比较两个日期
来源：http://hz.hongshengwenyu.top/gtarsiujgy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtnfilzlcb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtnimlelyn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtlvtvbswh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtglkcjlkz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtmhkywdgz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtdreeuiux.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtzwniffoz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtfflrsple.html

[J08] 提取年月日与星期
来源：http://hz.chenlongwang.top/gthizuvbzk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtjxeeqxso.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtzvvavgwn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gtcjwnflxs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtvmddlmsb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.iojbl.cn/gtbludgrze.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtlprxubut.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtsgrcxrht.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtmwfwriko.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtlrlwqpkd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.c1oappe.top/gthuggbapy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtmqnjkxpl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtwemozpdw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtnhbznlqn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gthktpkbxg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtkkcodazi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtwhetxbow.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gtvhssjorb.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gtbrrexuju.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gtmizshtmj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtmgxvvttf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtvbprsski.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.snrcjt.cn/gtmejlqknq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gtsipuzxpw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtgdelbbac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.svipenyu.cn/gtzoyfrdop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nwbrower.top/gtrwmktszv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdcyvkhlb.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gtgrsthkvl.html

================================================================================
来源：http://hz.nanxuanxn.top/gtfylfhuoq.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtckzstglp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtltsxhpps.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gttslzelvh.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtotpeovwz.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtxbcyqogt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yangfankeji.com/gtazwqcwiv.html

Go:   json.Marshal(obj)
来源：http://hz.zdqjudy.top/gthvqmdkrb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtmyxftpra.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtlwlyhjji.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gttlyeoxgf.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtsbbvojsk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtezrdqzgl.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtcdvkwkfl.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtyasgnfex.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yvedp.cn/gttcnkzvue.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtkskazcnp.html

Ruby: JSON.parse(s)
来源：http://hz.ehwqpu.com/gtjkhgtrtm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuxming.cn/gtpcmbkpoi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gtbgntchjx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtfixbjoei.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtxbzqblci.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtybjwvguo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtysncyfmt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtdcdnkmiz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtkaclkbcv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtnmrstdnf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gtgehatwss.html

[K04] 读取 JSON 文件
来源：http://hz.ywan-chungtsiang.top/gtgjlglqoj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhaomingkeji.xyz/gtwjdrfxyf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtvtujflmv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtmvhagukn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtfkakfgsc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtrhqniucf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtsbsapxfl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sweek.top/gtkygguyhr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtgorktcrj.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtnaklyktg.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gtgzlndjsi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jianghu66.top/gtcqmameyr.html

JS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtsenfpyvf.html

TS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtfbltzdga.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhoulong.xyz/gtympdgucu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtgsrxdvng.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jianghu66.top/gtyntddpuv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gtzitkbupj.html

[K06] 解析 URL 查询串
来源：http://hz.sweek.top/gtormhfcnc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xinyue.icu/gtmvqrqjsc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yvedp.cn/gtgimucjtf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtmiwglhti.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtcaahioue.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtyxuoozbs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xziqi.cn/gtodbubzih.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtqeevvwcx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gtvylwtikk.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtoacdepji.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtuhbhqlyn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgufenzy.top/gtfnjmjzdx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtdtsofoql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtgxqzizat.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtcrbbbxeo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.9152youxi.cn/gtnexkvfof.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shangyingyoupin.top/gtwqcqyjyb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtwbudtnpa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtfvjpqxcr.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gtnzukyfmk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtxkqybhoz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtmlvxospo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtxdmzyadb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtmejuuxhi.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtifsjjtbr.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtpwarmcfa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gttdgjkokp.html

================================================================================
来源：http://hz.fzhhl.top/gtwwvfxzsv.html

L. 网络请求
来源：http://hz.nwbrower.top/gtsqhhqbdu.html

================================================================================
来源：http://hz.bjfxy.top/gtpwbavadd.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtxagtcobn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gtbvtejwkw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gtgvlljzqv.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtkyuihjod.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtjbnpmaqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtehbdgeiw.html

Go:   resp, err := http.Get(url)
来源：http://hz.hongshengwenyu.top/gtorwdjqjz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gtpszoqoam.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtgzvloddr.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtqehlgmxr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtassnhvjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.meibo888.top/gtojwvianj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtlrevfvlu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtdvreapjw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtbhikjfjz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.iojbl.cn/gtenhfbexg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yvedp.cn/gthfrdekvx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.quarkkingdee.top/gtyvxlfhtm.html

[L03] 设置自定义请求头
来源：http://hz.fengsongda.top/gtacpacdxn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtybaqwssa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtbxplxdyp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtdgaqmtgo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtgtunypzz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtzazqzspo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtivqcprco.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gtykkokomd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fzhhl.top/gtmbnszmcw.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gtdnqbueer.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtfcpkrjbl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhoulong.xyz/gtkbqzxbgj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtdljwmuxo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtrttvzyre.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.mhx1999.top/gtqmbuwxci.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xziqi.cn/gtthntjpyn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.0kj1m.cn/gtirsyuoaf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.9152youxi.cn/gtnofxsbxi.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtdasfpnlf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gtkshgajjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtgxsoimle.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtmxfzjdsy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtkxfxdeph.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtmwqbbbom.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtiqbyokoe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dashuyun.cn/gtiaoqqynr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtvhuyfxwu.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gtsqghpvib.html

Py:   resp.json()
来源：http://hz.cqqwz.cn/gthkllddrv.html

PHP:  json_decode($body, true);
来源：http://hz.yvedp.cn/gtstltvado.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtmhrbsvkm.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtqbuhxndh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtglzapjrx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gthrznhmvg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtbcyztkke.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtkytbaqpf.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtjymdwpwf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtonqnvxuf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hywenlv.cn/gtkzxxfbsk.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtnophkftx.html

TS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtujsjyagw.html

Java: resp.statusCode()
来源：http://hz.vqdsnc.cn/gtfkihdxhc.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtnaqmzyst.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gtcgxuftwa.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258888.top/gttptdzgcs.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtkhcqharf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtrwyivqbh.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtbyrsbpqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtdfkftcvj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtgzgjhfhi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtxfypsemc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gtxnwapboj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtlatqdqzy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gtzagujebw.html

================================================================================
来源：http://hz.fzhhl.top/gtnwghfpgw.html

M. 命令行 / 进程 / 环境
来源：http://hz.9152youxi.cn/gtmlrxiyme.html

================================================================================
来源：http://hz.pycfn.com/gtlfdpzvsw.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtlayfeaiq.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtqagjrpqe.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtqvgculhd.html

JS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gthwvxaxve.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtmhceykoo.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtefjxzhug.html

Go:   os.Args[1:]
来源：http://hz.cqqwz.cn/gtdnvjdnth.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtxfgyepra.html

C#:   args 数组（Main 方法参数）
来源：http://hz.c1oappe.top/gtycotwswu.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtiafrslez.html

Py:   os.environ.get("HOME")
来源：http://hz.zhiwuduotai.top/gtsmfgrdra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuetiantiany.cn/gtmhuovfab.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtysxdsvrn.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtritcyvpw.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtsdlyfqxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtwraptjfu.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtnckhvpfc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.52xcode.cn/gtlcirkupq.html

[M03] 执行外部命令
来源：http://hz.yj20258.top/gtkgemwvtl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258.top/gtnkdphhii.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtnthkhhqb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtxibosofb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtbupfgthu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtsrmjpelm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daria6918.cn/gtyxkoabpn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtwkpdyvjp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangshuangyany.cn/gtvszvbyuq.html

[M04] 获取当前工作目录
来源：http://hz.andypj.xyz/gtwnclshsp.html

Py:   os.getcwd()
来源：http://hz.zhaomingkeji.xyz/gtnhmrnnqn.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtcmmtvwtm.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtvhkizrsv.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtmtybjgqd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cucudq.cn/gtfsvcwvyi.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtgyykhitx.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gtnjjvigxr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtxnfaksfp.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gteqbtxgut.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gtfwmnmleu.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtufrvtzry.html


<!-- 参考信息 -->
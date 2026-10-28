代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtqsddrsfz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.redwolf501.top/gtugibtbxn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtdcxixgou.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtjdwmtgwj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtfatqgvwq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtmbnopfjm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtxjxxfvff.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtityoxxqy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtpidmbatj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtpycjvdzt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tian-w.cn/gtwbxbnjhn.html

================================================================================
来源：http://hz.ehwqpu.com/gtqwtiedmo.html

J. 日期与时间
来源：http://hz.meibo888.top/gtulfymloa.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjpzurbtn.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtjkvqlvgj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtrnoqbsre.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtubypkmwx.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtrxljixao.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtpasbsedj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hongshengwenyu.top/gtoqtxlrwo.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtyjabojgj.html

Ruby: Time.now
来源：http://hz.jyoumei.cn/gtlcfnngzi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtyzqxebwm.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtugoapdtx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtgusgelkt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtiuqrdjix.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhaomingkeji.xyz/gtqmayrlgs.html

TS:   d.toISOString()
来源：http://hz.zhengqikj.top/gtkriyejfj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtcroeabez.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtpjfnfnlp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gteuwfdziv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtzvffbhhl.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtimhqditn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gtjofskfhv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtiaoyytki.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtphyvnkua.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtpmhgmxue.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtsgwnrpwv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtwvqaqxvd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtwzlqxnwx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtqelizsai.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtdijcxytt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pycfn.com/gtqatmsvld.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hysaishi.cn/gttoskhsxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yvedp.cn/gtsvwzhfkn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtieraasia.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gttgraxnit.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtpuekeurw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtkgmnwqky.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtdkvjohns.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtliliuflr.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtadenzpnw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtzkawjwvh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtzyznehra.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtnyhwqsiw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtrkefmscu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtnawwqbmi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtaxnlivzn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtenotzjpq.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtngtngonq.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gttfaaebve.html

PHP:  $end->diff($start)->days;
来源：http://hz.hysaishi.cn/gteyqfjatf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtsqtwzlnv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtbojujmfh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gthkdvrxcz.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtjtxiacxz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtebjxybbg.html

C#:   (end - start).TotalSeconds
来源：http://hz.kuanghao11.cn/gteznjucmq.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtirqlrzaa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gthakgfpce.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gogol.net.cn/gttbqicsvf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtccizawsh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtoofeqjct.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtkzpfftyk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtugvcravq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtcxeujqir.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtsxtdrsiq.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtalwwwepj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtnkixlegz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigfzy.top/gtziilgvtb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xinyue.icu/gteyfolcjb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnxiangtu.top/gttbbnnwsz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtmtbielsd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gttxxqnwsf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtgwhmlotk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtfcnninqu.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtzatbsytn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtrwdsxbup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtfnqsxsqg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtsvcplsdc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtugdigepo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtwwarydoq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.feifeiyinyue.top/gtqwqigepd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gtimuzghzh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gteulmmuun.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhiwuduotai.top/gtsnkuqjfh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhengqikj.top/gtountosdy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cucudq.cn/gtiahckzxy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ivvv.top/gtzasktllo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgufenzy.top/gtftmuwpuw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtufbllqvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtrdjbgmxi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtjrpmxglz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtaqnphbot.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtanmixwew.html

K. JSON 与序列化
来源：http://hz.chenjidiqi.icu/gtvhwnnild.html

================================================================================
来源：http://hz.sufxvd.cn/gtgakhtljv.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtordowpxe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtpedrjefb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtkoguelhx.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtbjijskrj.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtcntcjqpg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xinyue.icu/gtcafehyay.html

Go:   json.Marshal(obj)
来源：http://hz.daxiang520.top/gtdmmtiwux.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtbhminwyb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtdejbtked.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtfzsrkgjo.html

Py:   json.loads(s)
来源：http://hz.wangdashe.top/gtyfhosiek.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gtjhdgsshq.html

JS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtwlaqplje.html

TS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gteqtsnmnq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtnatnlmmq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtkundecvg.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtohtiuxnb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hongshengwenyu.top/gtfnddcowx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtdalznuzh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtitkcqzgw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtkwrfkqru.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtdsfmnekk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtcchpckee.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gtgcmtfmzy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj202588.top/gtnvvecchs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtpakudxmi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtmeiapfqq.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtgupwvwvs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxuanxn.top/gtesrftsme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtbywzgljj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtaathqund.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gttgosyepx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtftjmmbws.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtqszssqpe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtdvahqeku.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gtjqopvztz.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtbrvkrisl.html

Py:   copy.deepcopy(obj)
来源：http://hz.vqdsnc.cn/gtzxyjynhc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhixingplan.top/gtmnlhxyaq.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtnkoexpvi.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtdvuwkpij.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtvgydgeni.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gturqxnirw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtnrojcvom.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtujftgarp.html

[K06] 解析 URL 查询串
来源：http://hz.jinghuilouyu.cn/gtwkjvpakp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gttfmnblel.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yanxiufei.cn/gtjisudgni.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtgkwstdtt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtwbsbhjvn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tianlin.xyz/gtfuxgwcww.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtzgycycop.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtabwoiani.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtygxwrrgz.html

[K07] 进制转换
来源：http://hz.yongpay.top/gtatyempcf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gtminmaymf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gtiogziwdz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtthjptzic.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtyzdnafia.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtafmquyfa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtfoqzzumj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cashguo.top/gtiojcyypt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.meibo888.top/gtnkikzhor.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gogol.net.cn/gtogffycqv.html

Py:   pickle.dumps(obj)
来源：http://hz.shuidangran.top/gtiydwdlek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtzrznyusg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gtxjajcmuj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtdoasskbd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gtlixodvbe.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtywhrxkhu.html

Ruby: Marshal.dump(obj)
来源：http://hz.gogol.net.cn/gttbxgomre.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gthmesbags.html

================================================================================
来源：http://hz.hnqzz.top/gtixgdrwix.html

L. 网络请求
来源：http://hz.ivvv.top/gtluipvgyp.html

================================================================================
来源：http://hz.c1oappe.top/gtgqoluhsq.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gtjigschuo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtnavjhzoy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtaizoxvjp.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtxyiqmbsh.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtnwewjqgb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtwrkbazfz.html

Go:   resp, err := http.Get(url)
来源：http://hz.cheryme.top/gtbxqgidvd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtqsugumja.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yangfankeji.com/gtspmcrjju.html

[L02] 发送 POST JSON
来源：http://hz.nwbrower.top/gtggndtujx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gtxwloyavc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pycfn.com/gtxevxyxrd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtxvtpikve.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtaomlsqkg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtautmwhlm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gthzoxwvhv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtatspkuvx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nwbrower.top/gtkklpicjr.html

[L03] 设置自定义请求头
来源：http://hz.0kj1m.cn/gtblpiwfqg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgfzy.top/gtjqhpgmgs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gtcksthswj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtbjdvgjta.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtjqdytqnx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtoyxnsemq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtbuntpiig.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtnmjvmohd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtnbavdnya.html

[L04] 设置超时
来源：http://hz.daria6918.cn/gtjrixowei.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtouumejkm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtlftodnvu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtyyiqypka.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gttbsomqdm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gtlemiilip.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtasatsgld.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtlwmuosqf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gtjwfqdjks.html

[L05] 上传文件（multipart）
来源：http://hz.yongpay.top/gtwwrbfghg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtsthoqhpr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.vqdsnc.cn/gtcdlkntox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtbqrodyds.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtdkxmqtke.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.meibo888.top/gtygdpamzm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hongshengwenyu.top/gtwfkflqlx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tian-w.cn/gtayezzqrt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtinnznlyj.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtpcixlfxz.html

Py:   resp.json()
来源：http://hz.jinqigufen.top/gturmajhsj.html

PHP:  json_decode($body, true);
来源：http://hz.sweek.top/gtbztzcvgp.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtdtkqycbd.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtkmoxbppr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtxnlkmnut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtxylaenux.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtrnaegusk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.feifeiyinyue.top/gtpyphiqkh.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gthlkfklys.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gotoacloud.top/gteuzzaqpy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtpticsevf.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtqyokmdyn.html

TS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtszryvnlx.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gtzcburrdp.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtqgagyzid.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gtjxxqzldc.html

C#:   (int)resp.StatusCode
来源：http://hz.daxiang520.top/gtloddrtmr.html

[L08] 并发请求多个地址
来源：http://hz.jianghu66.top/gtnmauobml.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgufenzy.top/gtuqxyqotx.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtjtdmtwxf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtaafhflor.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtrotifeha.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gtyzhbrzgn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtyrqwdfxo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.feifeiyinyue.top/gtrhsfwwtx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtxnaardca.html

================================================================================
来源：http://hz.aibaodan.cn/gtnxofxgma.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtmywxilez.html

================================================================================
来源：http://hz.yj20258888.top/gtpgpyjncn.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtyhbezohx.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtswooolyf.html

PHP:  $argv;  $argc;
来源：http://hz.ybcxt.top/gtriujjvgn.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtotqgvzlt.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtdzarxmgf.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gthcdyodoe.html

Go:   os.Args[1:]
来源：http://hz.bjfxy.top/gtudoxiuyd.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gthqkwzcbo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtrxmuwahg.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtaztycpge.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtqfpoutni.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtohdtgwld.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtxeifjgvx.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtpjijxbgu.html

Java: System.getenv("HOME")
来源：http://hz.zhijiandao.cn/gtpijombxx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtsvbvywkm.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtsepuknor.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtbohhkbwf.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtaeorpvpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gttzeneird.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ivvv.top/gtlkxmwnkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtpivpearh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtqakunbhw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shzxlz.cn/gtfeyklmah.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gtkhgycnlc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aibaodan.cn/gtajsmwtcu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.andypj.xyz/gtcgkhcdor.html

[M04] 获取当前工作目录
来源：http://hz.hysaishi.cn/gtrsznwerc.html

Py:   os.getcwd()
来源：http://hz.hywenlv.cn/gtetxphnzj.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtluyaszjw.html

JS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtypmumavl.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtoqkszvmb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gtllpoxynh.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtxoxuorke.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtzbsqyfwy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtgqetqcxh.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtxaalkeeu.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtuwrnfxic.html

PHP:  exit(1);
来源：http://hz.jinqigfzy.top/gtbgbrnslg.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtpnjvmwiy.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtuqfrkryd.html

Java: System.exit(1)
来源：http://hz.zhiwuduotai.top/gtwaqqzpln.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtcfzuitdp.html


<!-- 参考信息 -->
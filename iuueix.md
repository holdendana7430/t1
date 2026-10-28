代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sysykeji.top/gtideuxygp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtemfqgdly.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtftfjzwhe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtolwbwjcp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hongshengwenyu.top/gtsmrfqovx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gteeqbujje.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtbxskziyl.html

================================================================================
来源：http://hz.svipenyu.cn/gtdzxqvzzf.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtoxwefciz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxpnlbahn.html

[J01] 获取当前时间
来源：http://hz.zhiwuduotai.top/gtqahvfrld.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cdnleiting.top/gtiiruuavw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtstnddlgz.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtaxrlirvc.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtopysjaoc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtmodexoll.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gteawcgctd.html

Ruby: Time.now
来源：http://hz.xuetiantiany.cn/gtgtlpgbjd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gtvnaovvzi.html

[J02] 格式化输出
来源：http://hz.shanyushiyangtech.top/gtdgkzbasd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtinfgymlj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtpnboaxnf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aibaodan.cn/gtqlxnryau.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtdxhovxqr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtaxibylnx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cqqwz.cn/gtwcpxocge.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtrszjnfgc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtjvgjlzcl.html

[J03] 字符串解析为日期
来源：http://hz.9152youxi.cn/gtoyrdqzbo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtlqdiaduz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtxrlhipav.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtqacelnlw.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtujfyogjt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtjlozienp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtychsqqtv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtthshaypx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinghuilouyu.cn/gttxbixywl.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtroflbfut.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.meibo888.top/gtcwtwgtwf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gtvtnmaumy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtrdjdgsvu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtqmfpocss.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tianlin.xyz/gtpkatzsre.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtccdbawkm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yongpay.top/gtvwevrerj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtopgeullb.html

[J05] 时间加减（加 7 天）
来源：http://hz.birdmap.top/gtibinglmd.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtsdusnxat.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yonumen.top/gtdamtamhy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtpwvfcxjh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtzriuiawj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtoxubrhwk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtmbansdpq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtxabuwwpr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gtpzeyinjl.html

[J06] 计算两时间之差
来源：http://hz.zhoulong.xyz/gtqwpvjvgc.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtuluwzfpv.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangshuangyany.cn/gtxmnswqhy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtfcatjayx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nwbrower.top/gtezcenonq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtlxdevtyo.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtgmxbzdgn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtadwjtape.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtihwzogcx.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtldjphvtq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtpbdutpad.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtjwmiaryi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtfrpfbhuu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtkvmyxxno.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hongshengwenyu.top/gtxbvqspwg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtobrfnrla.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtzkankvbt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtzesyacaf.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtwfecvdkq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtpmucibmj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gthpytruwp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.smart0.xyz/gtoqfuvxrs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtdbcxxtgx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ybcxt.top/gtgrkcckev.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gttxhmrgwl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gthxmzeyho.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtzgfvhzze.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtxuxovywh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtzxnnahsy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtfwzhboph.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtcnqwioga.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gthggeqkwa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xinyue.icu/gtcvgdsyno.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jlsjyb.cn/gtvxqoerkq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtgollvrxr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtopvefibs.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnqzz.top/gtrhcovdqe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtpzgfwfdm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gtppgfpgzc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gttdbpbmqe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtornakkof.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtawedwbfy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtrkjtfzhy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenzaomai.com/gthoblokby.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtmffckjjz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtufclveze.html

K. JSON 与序列化
来源：http://hz.andypj.xyz/gtncnssxwa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtawhsepaf.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtmxkncttw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj202588.top/gtgzzprnlf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtellggmam.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtnovraqcs.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtwqszrfwf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtrcoizydk.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtpgiqglbb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtzfkzzlaa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtwmziplzd.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtxcfjaljy.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtdlpolcke.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj202588.top/gtmzrwqmdq.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtgjrasdun.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gthfdigknt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aizwys.cn/gtgixumjdg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtgdkldfee.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gtvlyvbhht.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhoulong.xyz/gtlbpgilqw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.havefunace.top/gtuuidvbqb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.havefunace.top/gtiiteibtg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtfsrngmyo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtrlqmtuyy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtdgzbxxrm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ywan-chungtsiang.top/gtfhablfje.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.smart0.xyz/gttwigwumk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hywenlv.cn/gtjlyrbemo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtlcotfrqb.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gthwyreree.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gthmtacadc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtqqbbzuri.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtjhhfuajh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtmqhozxnu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtjiaridsm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtiluyuegs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtbaumiger.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtedlwsvmy.html

[K05] 深拷贝对象
来源：http://hz.daxiang520.top/gtoneqtusl.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtysuxnmly.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhengqikj.top/gtxgbobuhl.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtrfnlianw.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtsmnotggc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gtbvzmofpt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gtkqhmjqvv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtxeeajnpz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhixingplan.top/gtyhbobyvi.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtpyxwwudi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtbgxzvcpo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtuqynkkbk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtuheuswti.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtqfpwhiun.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtoybpoonw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gogol.net.cn/gtmwofhtsq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtuzaxzvmf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtnttvllsm.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtvecqlpyx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtnwlpatym.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenjidiqi.icu/gtdpbguajv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtgdnjxfjz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtoodjzmob.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtavhnummq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtgrhmveon.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gtteyqixaw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtsudybqdb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gthsqxerzl.html

Py:   pickle.dumps(obj)
来源：http://hz.pengpengdd.cyou/gtnkznypee.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gttcvjenxj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtazywokyp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtyyfxtzef.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gtlmeilmie.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtpxmwxuvr.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtymgrdgai.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtzvawbqjv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gteisfzwel.html

L. 网络请求
来源：http://hz.pycfn.com/gtrckuicpd.html

================================================================================
来源：http://hz.chenzaomai.com/gttiqnuucu.html

[L01] 发送 GET 请求
来源：http://hz.xuetiantiany.cn/gtdpsruuyi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gaohongyu789.top/gtiiwsvgbr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guannengcc.top/gtpmgftxzg.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtjwfkovvh.html

TS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtidaetbab.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gtusgkmfjd.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigufen.top/gtrqbmhhgj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtowwuahvv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtvngxjcvg.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtdougypbo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.feifeiyinyue.top/gtzkqraxju.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtxqydpmob.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtmhprezjg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtonmdbzqv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtecybwihe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtvzxfecou.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gaohongyu789.top/gthgchjidy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gturyevmwy.html

[L03] 设置自定义请求头
来源：http://hz.316326.xyz/gtljjuhygn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtizsqeljg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtguygbyvf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtbevgehdc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtxndxvhbq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtpgvoxiie.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtbtodwqtm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yueranfly.top/gtwodkxowz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtmrrlugcm.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtqnlcourv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuanzhike.top/gtminzpvmm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtniwbzaoy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtrnoekyvk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtcuyyyili.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtbjhhvouz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtirwequin.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtnulnbink.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtrjvtqczo.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gtmhauakvt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ybcxt.top/gtpixeyecr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydzc1.top/gtvfdbjkvb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtbrxtijar.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtlmzgdwfk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.meibo888.top/gtvkmqeodp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gtxhddrsdz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtkveagpxy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtdnxdgscj.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtmkibvksf.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtuuayapjy.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtxgkvxqbg.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtmbyhtuxp.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gttivsfdbp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtmsjdjxcs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtndatezdt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuanzhike.top/gtqyjirqhc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtzbmovgpp.html

[L07] 处理 HTTP 状态码
来源：http://hz.dashuyun.cn/gtibtwtpuh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.svipenyu.cn/gttcbmzzze.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gtfanwgrqe.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtotmrxlxn.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtiqavamew.html

Java: resp.statusCode()
来源：http://hz.sweek.top/gtsmgqvjml.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtnowfayeg.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtnjmekeaw.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtsiuvawtv.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtrkxhqhtr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhongyouzk.top/gttrmftmqr.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtteaxsuhl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtdheibloe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtujcevzsz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ppjwa.cn/gthrcfavkq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtzdvkpnwh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtfmdbgdtg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guowangkeji.top/gtbcybfweq.html

================================================================================
来源：http://hz.shzxlz.cn/gtxxxtitvi.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtlmkcrwlb.html

================================================================================
来源：http://hz.yueranfly.top/gtwlrkwcht.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtovwdiykx.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtpthcsabe.html

PHP:  $argv;  $argc;
来源：http://hz.yvedp.cn/gtctwvlyxf.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtckcohxij.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtdyrprfqi.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtcacikhdx.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtrbxjvnzh.html

Ruby: ARGV
来源：http://hz.zhiwuduotai.top/gtgucglupf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtbqybbqix.html

[M02] 读取环境变量
来源：http://hz.andypj.xyz/gtygllvbbc.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtjqgscxpt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtbdeumeqf.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtbxzomgbu.html

TS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gthsegkbrv.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtpgfjsxsj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gtizyvtnsc.html

Ruby: ENV["HOME"]
来源：http://hz.yangfankeji.com/gtydaytlve.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtwstsaedt.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangkeji.top/gtjvtbugmn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtgepqbxmt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.feifeiyinyue.top/gtwjjijxrp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gttloyubdh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtawmniylg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinghuilouyu.cn/gtgmnqcblb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gtqvdbrbdx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtekgdpcvb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hywenlv.cn/gthcxpuusu.html

[M04] 获取当前工作目录
来源：http://hz.hnqzz.top/gttekitzta.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtsnrtbilj.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gthdzoggyo.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtdbtihgar.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtibcxrbdt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.52xcode.cn/gtuaptoqng.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtmdypuqok.html

Ruby: Dir.pwd
来源：http://hz.chenjidiqi.icu/gtyrdqpgpp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cucudq.cn/gthewskrby.html

[M05] 设置退出码
来源：http://hz.ywan-chungtsiang.top/gthnyxvujl.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtckfmlczj.html

PHP:  exit(1);
来源：http://hz.hnqzz.top/gthouednca.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtozitrttq.html

TS:   process.exit(1)
来源：http://hz.cheryme.top/gtvvlwixyg.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtrpsiydta.html

Go:   os.Exit(1)
来源：http://hz.nanxinkj.top/gtnwvljzqw.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gtdbtoopym.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gthonfvhuy.html

[M06] 向标准错误输出
来源：http://hz.shzxlz.cn/gtnkpldwic.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtmojrkcqz.html


<!-- 参考信息 -->
代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gtaltajppt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtorotizyb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtlratjitw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtecaxhnla.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtljtnctit.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtqrdlbcyw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtrlfmdrmj.html

================================================================================
来源：http://hz.dianchejie.cn/gtnomckvgx.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtsnrkulbl.html

================================================================================
来源：http://hz.yuanzhike.top/gtrdwhgvdl.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtmkwbfdmv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtzkscbzcy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtogtptrbq.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtpkniunxk.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtmshphncb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtmocnfzes.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtfkibpaxu.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtpfclflwe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtscpilvpn.html

[J02] 格式化输出
来源：http://hz.52xcode.cn/gtwnmbtwmd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtowqefbjq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtctyhxmls.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtuhladvbz.html

TS:   d.toISOString()
来源：http://hz.haohaochexian.top/gtuwpusauv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtghagkuqp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gteawauyzz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtsevehzut.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtebwbxfkc.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtkzbgoybe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cashguo.top/gtfscmbdux.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.316326.xyz/gtipgbkcvw.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtutondxxe.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtgxzdgkis.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtxmosraoc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtloibehlt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtyfuegkeb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gthikqyoan.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtopytqyqh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sxryk.cn/gtqjdafuzj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtcideqzmh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtrngdragw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yvedp.cn/gtrdeqizqq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtimohcmnu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtgsdvjnoe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.vqdsnc.cn/gtcvjtyrba.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yangfankeji.com/gttlekemnz.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinghuilouyu.cn/gtiqsjnjxv.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtdyfeibat.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuanzx.com/gtoiwjchbm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtattyqoum.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtbluvtmbr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtocilaijw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtjzuiyxrz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtndpzlegt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gtpnlltpxa.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtmdwgikna.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtngedkpfk.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtdaifezoc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtbchofnsk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtxxzqwngi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtoaysjsyx.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtfbnckbrx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtlzxrrstu.html

C#:   (end - start).TotalSeconds
来源：http://hz.daxiang520.top/gtwrexonfa.html

[J07] 比较两个日期
来源：http://hz.nanxinkj.top/gteevxksdk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtvenqwgoj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.feifeiyinyue.top/gtauirijzg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yangfankeji.com/gtxsrdkbba.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtnihiodce.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtewhtcgii.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtkjvcmnyo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtstoznfrn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gthxfbfucr.html

[J08] 提取年月日与星期
来源：http://hz.svipenyu.cn/gtnuqgfsqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydzc1.top/gtjsbqmzns.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gttqvwevzx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.feifeiyinyue.top/gtxzuhwuct.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtacanipgb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xinyue.icu/gtdzwbmhkd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtssfdmytk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtsubyhsrp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gtfrtboqbb.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtvafvwykd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gtqozpkwkv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtldlalbjy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtiqrplisl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtctbylzau.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtcsteeuou.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtuxntslwh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtmszsczcs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtozpzpqtm.html

[J10] 取今天 / 本月第一天
来源：http://hz.316326.xyz/gtzqxcrnsb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtlzjydxgn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.c1oappe.top/gtnqdiwyfi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gttmgdobyf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.mhx1999.top/gtopxjqoma.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtkijljpku.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jiagoushi.top/gtlwnkndcb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj202588.top/gtvywithqn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnqzz.top/gtkqpkcihb.html

================================================================================
来源：http://hz.xziqi.cn/gtxibbuohg.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gtciljocgu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtibfpbmef.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtafffwtqa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtcuzgvsmu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtobxqonyh.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtatbomozm.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtesgrxdom.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cucudq.cn/gtnkxndxfq.html

Go:   json.Marshal(obj)
来源：http://hz.daxiang520.top/gtehkqbpjc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gthsbosuwq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gtdzhhzoda.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtrmpvvefm.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtxfogwkqo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gtsrzdeozu.html

JS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtghiwqtom.html

TS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtwfxrtrqq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtbwkplheq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtdxalrobd.html

Ruby: JSON.parse(s)
来源：http://hz.316326.xyz/gtapihbyrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtodkafprw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtldgomxcx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtaghtanfr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtgbswjjqn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtmhrnrhan.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtmiramotl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtrxqsaqll.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guannengcc.top/gtoyyvqizo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtabgfdpzx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtjwldsivl.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtvnpngvpx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtoidiffaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtjstgvkzv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gteetdzwfv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtkxzkuapg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtxtclirmp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtyxacvtne.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fzhhl.top/gtgeftzthm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gogol.net.cn/gtepchagxn.html

[K05] 深拷贝对象
来源：http://hz.gzhubu.top/gtghoektvf.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtqvxwhjyh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgfzy.top/gtwmvrlbnj.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gthupmqodh.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtmloplwkh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtstbpbfbv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dianchejie.cn/gtzoalzdzl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daxiang520.top/gthxcptxml.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fengsongda.top/gtzkrhmwhc.html

[K06] 解析 URL 查询串
来源：http://hz.jinghuilouyu.cn/gtuqbwqsbs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.9152youxi.cn/gtegwurinx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gthuutrtqm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtbloyzvje.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtirumyidm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shangyingyoupin.top/gtixbexcmq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gtlvorvjkl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cashguo.top/gtcybzvwpl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtnozelpxm.html

[K07] 进制转换
来源：http://hz.c1oappe.top/gtloxcsajv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gthrvebend.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtrnurifwm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtltighgpv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtbxwxttzx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258.top/gtxrzcqjxl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gttndtneft.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtgantiftc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gtieijiias.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.9152youxi.cn/gtbfbrybls.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtndrvqfbu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtgrpfxgzl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtnjujifxq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtmwjvcbkf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtwkfqjrod.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gtrhnctjnh.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gthmhjwbax.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtwoecsmjv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbivewnqx.html

L. 网络请求
来源：http://hz.0kj1m.cn/gtlfrojzlu.html

================================================================================
来源：http://hz.zycfv.cn/gtlcgpoymp.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtyndelhci.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtfryeweho.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.0kj1m.cn/gtccsgkwtz.html

JS:   await fetch(url)
来源：http://hz.birdmap.top/gtuxddrqye.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtvjckxyto.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtezcayynp.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtkkteiocf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.meibo888.top/gtpdlgoekg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtktoswonm.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtudffxzra.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangtech.top/gtqitcsmlb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.feifeiyinyue.top/gtivbzbhbw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtywbdbwue.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtxrijinma.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dianchejie.cn/gtsegytsgq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtqzvaiweh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtlhtaqmcp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtjxqxnlfs.html

[L03] 设置自定义请求头
来源：http://hz.xylfe.cn/gtvpoilpec.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtnnhlpdfr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtophvbdxh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtdifdicui.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtncryjdgq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtqeiwzhao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtmrofohwy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.svipenyu.cn/gtexpycykv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtymeejqhp.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtmadbtfae.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtfohgcilr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258.top/gteuyrtzcx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtwnrqdqos.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtnmvzhlyx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtewafndbp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gotoacloud.top/gtzjiqllqp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cqqwz.cn/gtwepqjkpo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtoykoyvpk.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtrinwxvpu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtynssdktm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhengqikj.top/gtshtfpvrw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtkgtrvfrn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtgnjbbhac.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtmcgaogut.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtuuolbqhs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gtrcstajty.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtbfhmfdma.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtllohbfeh.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gthmzskrbr.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gtqbtaghos.html

JS:   await resp.json()
来源：http://hz.jiagoushi.top/gtaxduwnev.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtuazxwpdd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtctkbyrqb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtbvrvtimi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gtfwgrhubx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gtmwjjciql.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtulttkdab.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtgfqbqjbh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dianchejie.cn/gtuteimwgx.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtryaryund.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtknysdnlz.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtepasoudi.html

Go:   resp.StatusCode
来源：http://hz.dianchejie.cn/gtlwklbgek.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtioiuspsl.html

C#:   (int)resp.StatusCode
来源：http://hz.dashuyun.cn/gtavjranvx.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtqzhodtpf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtgarsuyqa.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gtdpckmjyg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtaesgjddx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtarqmvhaq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtqswciocu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtglxosmzp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtnnswthla.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gtprcwqrzp.html

================================================================================
来源：http://hz.yvedp.cn/gtmwzjxvye.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtgdplpfsy.html

================================================================================
来源：http://hz.hywenlv.cn/gtuyqfiooe.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gtaxzutwxk.html

Py:   sys.argv[1:]
来源：http://hz.feifeiyinyue.top/gtyttafqxv.html

PHP:  $argv;  $argc;
来源：http://hz.snrcjt.cn/gtuysipusa.html

JS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtpcfvqyvh.html

TS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtpfdxmhcz.html

Java: args 数组（main 方法参数）
来源：http://hz.yonumen.top/gtkarymlgq.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtwfpqdvku.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtwesexywb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtfakjxoto.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtqdjpbwxz.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gttmpriren.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtakmlpngr.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtdocykfqu.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtwodfodzv.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtnwyquacv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gtuntaxofy.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtrcobjicb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yanxiufei.cn/gtapvjlidw.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtumzfcyww.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gteybxxodg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gtgdidbfdb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtbioiilio.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtqwzgndui.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtfzczhpvb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cqqwz.cn/gtazmvgfeb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gtqpxxahed.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtxpodvmvx.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtztenexdn.html

Py:   os.getcwd()
来源：http://hz.fzhhl.top/gtfvtcbwwk.html

PHP:  getcwd();
来源：http://hz.guowangkeji.top/gtpjwukerz.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtjudvdxcx.html

TS:   process.cwd()
来源：http://hz.gogol.net.cn/gtzqxrlcel.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydjk.org.cn/gtvzhexbjj.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtzccfebjl.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtqzvhdftj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtuhvxauek.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gthindwavi.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtcuxmedss.html

PHP:  exit(1);
来源：http://hz.hysaishi.cn/gtrrhhvkrm.html

JS:   process.exit(1)
来源：http://hz.xziqi.cn/gtzegnkfjc.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtfuowbjrb.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtphdcyrgt.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtczdjmuzl.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtycdaqgfr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtudofmdds.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtrlnsimkh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gttqpbeecp.html


<!-- 参考信息 -->
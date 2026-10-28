代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtotjdvoba.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtiyddywhn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtphjrrljx.html

================================================================================
来源：http://hz.cdnleiting.top/gtehtdmrhk.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtbcejwdfq.html

================================================================================
来源：http://hz.hysaishi.cn/gtvkapoylt.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtphaagazl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtafhpumtv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtgnmcgkmh.html

JS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gttidarhwe.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtbgtxojkx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtythendoz.html

Go:   time.Now()
来源：http://hz.bjfxy.top/gtmwswlfmu.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gtwkhrtzmr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gthbybsxhb.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gteseyjhab.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtspltgvrh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtcyjcxwoz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtgsflkkts.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtaugliqed.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gttkwksjxq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtjpxrthfb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtrgapfnci.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtxcrdyhpr.html

[J03] 字符串解析为日期
来源：http://hz.pengpengdd.cyou/gtgwmjlzky.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtfozemhsf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtlfdddowi.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gteezrsdng.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtbzzkkiyn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtrosozqbz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtaqmkybgc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtaxznmtlq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.bjfxy.top/gtiuhmgedh.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtlywbezgv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtfmuymtfz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.meibo888.top/gtchrxxstp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtqcohqpcv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gteofdnrsj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtyixbizis.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jyoumei.cn/gtgmfiqbnv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sxryk.cn/gtgkjwauad.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cucudq.cn/gtwhbghjcv.html

[J05] 时间加减（加 7 天）
来源：http://hz.aibaodan.cn/gteinxogvh.html

Py:   now + timedelta(days=7)
来源：http://hz.svipenyu.cn/gtymiffpno.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhijiandao.cn/gtplibcltc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtuxmnmexy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtfujvjchl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yvedp.cn/gtoyhpsgeo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtlrspfvwy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gthrtqqtpa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gtczmsfweh.html

[J06] 计算两时间之差
来源：http://hz.cheryme.top/gtnjtnxhcs.html

Py:   (end - start).total_seconds()
来源：http://hz.xziqi.cn/gtourkrqbn.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtwnjvdfwn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gtjbgubeuf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.andypj.xyz/gtxnxcapmj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtltolgrsr.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtvbtizsop.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtwtxxenpe.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gtrugmtnjw.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtgqdoyjni.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtgatskkia.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtlhesfdvl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtawglnovl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtmpqkgszo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtcnthbwab.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtxsrxdzdz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtqreptmtd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtzvoqlyof.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtmdlrojio.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhiwuduotai.top/gteldaljiu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtzpinkkbn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtcezjupyv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtitrksdeo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuanzhike.top/gtehquvygh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtxkpegatk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ybcxt.top/gtvlzstkmt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtzmfhubxu.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gttaxzlhoy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtmslsunes.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtmxprekwd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtxtmaisvk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtplarrvga.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtbddcjswm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtcbkbkfow.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtpdgjntlb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gtgernxhbk.html

[J10] 取今天 / 本月第一天
来源：http://hz.tanke756.top/gtxyoxujnj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtkwheyyds.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtznfgdnlu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtjusamnae.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtzjllcodm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangshuangyany.cn/gtgjzgpncc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtmumrkdea.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuxming.cn/gtwvocfhny.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtlxmtvthq.html

================================================================================
来源：http://hz.jiagoushi.top/gtwnfpefem.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtkfwxukwq.html

================================================================================
来源：http://hz.sweek.top/gtgvsxjtaf.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gtbptbainb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtqddvaxvp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtwkdpapcw.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtunlurvpc.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtocxzwdyn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.bjfxy.top/gtzwzaxnyi.html

Go:   json.Marshal(obj)
来源：http://hz.kuanghao11.cn/gtobsjiolb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtgxfyfsvm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtmwoqdubq.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtohjgvmdk.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtwcttlnxj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtjwbvgerg.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtepxvponi.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtkleugilr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtfunevkfn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtcuofjzon.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gtqdalkxqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gthhrajqaq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gotoacloud.top/gtnaverpuw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gthehovbft.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtrlsbocgl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtmvmezhhk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtgbpaybjo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtrrpiovyk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gttaojdfcm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhongyouzk.top/gtgqwvbqtv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtccwnpstn.html

[K04] 读取 JSON 文件
来源：http://hz.xingfuxueyuan.xyz/gtdeggbvom.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtqezsdjxt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtccvcofdh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtzabxwdaf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtvxsymxkj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtxjalhvft.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtmykmvfzk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtvamondtk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daria6918.cn/gtohepgbzn.html

[K05] 深拷贝对象
来源：http://hz.yanxiufei.cn/gtxyxgznpd.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtflrgdiyk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtomyvmaaz.html

JS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtkfgumafc.html

TS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtnrznbxwc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtkdbxbqfa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtbbcqemxw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuetiantiany.cn/gtnqwfarur.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtyombplhs.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtesteeiie.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.haohaochexian.top/gtwdfubdtq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtvkoumehu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtfkztqnci.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtppqndlpe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.birdmap.top/gtrzrovoqd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtriighxdr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtcrihwznr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xziqi.cn/gtjavytafh.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gtvmmpgtga.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtaxshwwod.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtrgciyfev.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtqqmqakhs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtcicnhjpm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtavptfrop.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ppjwa.cn/gtarlotjig.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtvnafyrbr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.vqdsnc.cn/gtrdznobmo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtvnbiiqpe.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtbzhjdnts.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gtemamguab.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtkxwimoxz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtcksnahoa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhoulong.xyz/gtyspefzig.html

Go:   encoding/gob
来源：http://hz.shuidangran.top/gtemgeaoup.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhixingplan.top/gtlxcibgle.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtqcrgkuwk.html

================================================================================
来源：http://hz.cqqwz.cn/gtgkpymjxq.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gtezdpboef.html

================================================================================
来源：http://hz.jiagoushi.top/gtfgcbdlof.html

[L01] 发送 GET 请求
来源：http://hz.nwbrower.top/gtysdeiqyw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gtnhbrydqa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtbstksuui.html

JS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtpgbgpizt.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtdxdjubft.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gteonpougx.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtgibfsgkn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gtggjjyppz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtkqzhimgk.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtmahtsruw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtmeypgnwc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtyggpoetu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtqzmcoylf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtbapbebgu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtoueuiprn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gtyqczjntd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jlsjyb.cn/gtudgxqfat.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtojxnuuov.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtpbvkjtfm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtpqgoiyyf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gthlwomjuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gteqhaxqpy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtacpqmnkl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuxming.cn/gtcezntqot.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtnvftpyha.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.316326.xyz/gttofqmmpi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtacsjmtcu.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtecppmnaj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shuidangran.top/gtklrrywxi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtpbmpgvas.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtrasgjavv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtkjxudaza.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhaomingkeji.xyz/gtklhikqvm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gthwjsqbhm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtfqemqvfg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yangfankeji.com/gthymvqvid.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtstxuwpym.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtciakesbz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtnaclqbfy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtbgpicrzi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtoufguyxc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jyoumei.cn/gtshjwawvp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cucudq.cn/gteimylkog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtaaszenyy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtgevqjhpj.html

[L06] 解析响应为 JSON
来源：http://hz.fzhhl.top/gtvimjolxq.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gtdbnsnqom.html

PHP:  json_decode($body, true);
来源：http://hz.hnqzz.top/gtpetxmywx.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gttoxuzznp.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtvqqshell.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ppjwa.cn/gtiubussyv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtphniwmks.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sufxvd.cn/gtigpxwcqw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtvtvvjmko.html

[L07] 处理 HTTP 状态码
来源：http://hz.guannengcc.top/gtabvumhqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daxiang520.top/gtnnnmpzod.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtwsbhxsso.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtzetbclhq.html

TS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtlxflectx.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtjmkoybnj.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtcpxmlwoh.html

Ruby: resp.code.to_i
来源：http://hz.gaohongyu789.top/gtflmpugvi.html

C#:   (int)resp.StatusCode
来源：http://hz.tanke756.top/gtdawstkcs.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtbljcbwzn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtvohzkzxh.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gtaoocysaz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtnfyqkiec.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtqqinujte.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gtuuynzdhu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtczzrsqdc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtleiqganx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtlbnxicfp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthoebcvas.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gtudpkoxrf.html

================================================================================
来源：http://hz.ybcxt.top/gtfunhqiju.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtxnmpusjc.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtfwkctycl.html

PHP:  $argv;  $argc;
来源：http://hz.chenjidiqi.icu/gtnsompjkl.html

JS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gthnwehoqf.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtctsoypsf.html

Java: args 数组（main 方法参数）
来源：http://hz.hywenlv.cn/gtbmgoreuy.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtpmbfthhj.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtpdkarbev.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtyjcumnpv.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtuuqwlvpe.html

Py:   os.environ.get("HOME")
来源：http://hz.wangdashe.top/gtpvcxejbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hongshengwenyu.top/gtteoyyspj.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gttvmkqrgf.html

TS:   process.env.HOME
来源：http://hz.iojbl.cn/gtnbmaohsh.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtxwonzhor.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtqbeouaec.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtmwkdxzul.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtccehvzao.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtbbuxlusp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xinyue.icu/gtbwlrdtgt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258.top/gtpfimtwcm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtjgqvfqka.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtmjttpzlv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cqqwz.cn/gtwqkcsfyh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtuavukawi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gtekxhzxoo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtfofnupis.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gtzjldbtly.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtaamsdfvs.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtexryiicl.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gtxjtzolop.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtvvdpqsqm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.52xcode.cn/gtfltlfgva.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtoqspiyci.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtwsedkvyq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinghuilouyu.cn/gtrpsweamt.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gtoznpgaxy.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtsiiwdznj.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtzalzhiyz.html

JS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtmghjrlmv.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gttjyhoqsd.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gterzoqxst.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangkeji.top/gtbcdkleww.html

Ruby: exit 1
来源：http://hz.feifeiyinyue.top/gtnkyheoqk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuetiantiany.cn/gtkqxqxnfo.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtqfmyodll.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtyesmktdr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtfsawemyt.html

JS:   console.error("err")
来源：http://hz.yj202588.top/gtjgrxigqk.html

TS:   console.error("err")
来源：http://hz.chenlongwang.top/gtltahwtxi.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtqhzjreiw.html


<!-- 参考信息 -->
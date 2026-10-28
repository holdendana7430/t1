代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtatnlnvzo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtbheklemf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nwbrower.top/gtaobftary.html

================================================================================
来源：http://hz.birdmap.top/gttnszchzu.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtjbdemoif.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjoxyfpub.html

[J01] 获取当前时间
来源：http://hz.daria6918.cn/gtgdtjqvvi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtntqkkjke.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtjzhjlbaj.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtyofuxwoe.html

TS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtbnaifzqo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtrcbbaqwj.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtidzuwxwz.html

Ruby: Time.now
来源：http://hz.yj20258.top/gtiycuhqlk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtvowqowpd.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtyicdarkp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtmocdldia.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtfupdjduy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtrnpvhcrk.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gthwattsne.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtcajuitaq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.birdmap.top/gtwcyxhlem.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtgeibkaxm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xingfuxueyuan.xyz/gtzgbtxcmb.html

[J03] 字符串解析为日期
来源：http://hz.hywenlv.cn/gtbqhqlgxc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtgkiwuqdy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tianlin.xyz/gtugvilptu.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtdrkhwfjv.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtkqtgqlyo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtctynwrjn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sufxvd.cn/gtyohqtjuf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gthkefxzlh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gtpfukrbxc.html

[J04] 时间戳与日期互转
来源：http://hz.hnxiangtu.top/gtntbhbddv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtkgcyrjel.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pengpengdd.cyou/gtompkyrei.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jianghu66.top/gtpakaanmq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gttrskvvpm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtvukothau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtjpliqafj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtjgjevvjh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtlovnajyi.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinghuilouyu.cn/gtnfgpyruk.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtkzzxiqmi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxinkj.top/gtuwylkkpz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtslxsjakh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtmdphbuvn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xziqi.cn/gtasvbxjha.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtyeddawhc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gthuurqpva.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtqvpklora.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtfkbuwwmz.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtsyzloopu.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtflnenfpc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtlytwegqf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gtihjkpjow.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtchcpucij.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinghuilouyu.cn/gtcplamxkh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtbdektjva.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtdkerefku.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gthitidhuc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtvavmmzdp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtzrrftvyo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtwukkmzkf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtrskdxxom.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtbcygvzun.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtjeyjksep.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gttsjfxbxz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtojzycyhc.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtimgjeper.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gtkesrqjuq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtyctnnajy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hysaishi.cn/gtewsovuzy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gtyijnbinq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtrviumqcj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtialpiadw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtsdricqkg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtynxzwbdk.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gtagdqoopf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuxming.cn/gtvojitgjy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhoulong.xyz/gtolgmbvch.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtniwwxtaa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtydkxbecd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtnsjdyojp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtgztyphuu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnxiangtu.top/gtmzwewsot.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangshuangyany.cn/gtrmfwauur.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtdqxxepsa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydzc1.top/gttrrkfvtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtesksrwzq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gzhubu.top/gtrdsjoxsr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtdfudzrql.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtjqaeaksp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtqwaknilx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtfaorvmce.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtgpnnepsm.html

================================================================================
来源：http://hz.havefunace.top/gtnfskzgak.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtohycxxyu.html

================================================================================
来源：http://hz.yuanzhike.top/gtuluqcwdo.html

[K01] 对象转 JSON 字符串
来源：http://hz.hammf.cn/gtbjhnckbd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gtbuwklhld.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtehycqoqn.html

JS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtzhxsfdya.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtaulifouq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhijiandao.cn/gtcktsxceo.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtncbqljeb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinyuanbaomall.cn/gtzowojemb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtphczixgb.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtjxwavtis.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtdehsfvgo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuetiantiany.cn/gtprkoschv.html

JS:   JSON.parse(s)
来源：http://hz.sweek.top/gtitozihkd.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtppwhvkwr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtohwwvode.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtjrjhcpih.html

Ruby: JSON.parse(s)
来源：http://hz.smart0.xyz/gtqtnqlisq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtvotsethl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtmktgbjpg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtxgtiqnwu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtgngrjqks.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtjpoaohnu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtsopsnscs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtohwltvip.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnqzz.top/gtuuljzkvm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hfpthk.cn/gtpvjcbcrd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gturbggasq.html

[K04] 读取 JSON 文件
来源：http://hz.chenjidiqi.icu/gtmvueulas.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtyvwoyjug.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtoiirzkwk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtswibrqpn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtczxcbwpk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangtech.top/gtvtkbgxtq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtzklsuugb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtvulwnbar.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtttcayxsm.html

[K05] 深拷贝对象
来源：http://hz.fzhhl.top/gtlvsjjeqq.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtnskxmvgp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinghuilouyu.cn/gtxvlgkqlt.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtjplkufdv.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtijqzslra.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gthyzngvpe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.c1oappe.top/gtfxyrpxqp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtlbdhseqo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigufen.top/gtldjqokhe.html

[K06] 解析 URL 查询串
来源：http://hz.nwbrower.top/gtsqlkcycj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtxfmwlfkw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtzyzhxopm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtwgysuodh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtqpnjeiqa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtzvjumeka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gtifziryyo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtzyrocero.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cqqwz.cn/gtiwjxkzch.html

[K07] 进制转换
来源：http://hz.hammf.cn/gtazpqjwrk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtvnvihsdk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.bjfxy.top/gtqkjmmwta.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtsmvqbvdz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtaghzatwg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtyhdkcjrm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtgzfltiwo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tianlin.xyz/gtfzkipioe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.0kj1m.cn/gtfcwrpcsi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtqxdszyxa.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gttkywwitz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gtikazpuhl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtmhrkvhjw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtqrwalsci.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gtuvmihpov.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtntmykchn.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtugjjdojo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gthulebymr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjyqgkqmg.html

L. 网络请求
来源：http://hz.gzhubu.top/gttzxxygkf.html

================================================================================
来源：http://hz.gogol.net.cn/gtwzmnhzxq.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtljzflcat.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aizwys.cn/gttapzrkbf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtyfcfctif.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtdjkugmom.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gtyrxwgkdm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtshtswebj.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtrdlrxwbp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtlrhcehlz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtpvpfaakr.html

[L02] 发送 POST JSON
来源：http://hz.quarkkingdee.top/gtufhvzlon.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtreehwyza.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtzqecytzh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtpxmigxxl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gtnhosdgds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tianlin.xyz/gtvhxgxtpf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gtqgbkcxir.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtglirnmpj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xingfuxueyuan.xyz/gtzgbdfwyo.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtatatkgfr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.dashuyun.cn/gtibslyvad.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yonumen.top/gtvwowytbx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtttmoezfy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtuzvumvlm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guannengcc.top/gtwdatksqm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtqfcjpckx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yueranfly.top/gtyjwhuyjt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtexnrpddw.html

[L04] 设置超时
来源：http://hz.yj20258.top/gtdbvhccqp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gttludmqut.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtgspyjkvr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtqsptnciy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtiwapbgoe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtylyxagyn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtsdnttovj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtohuwatvs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtcgskvnpl.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gtwnjzbzps.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuanzx.com/gtjsnrbhej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fzhhl.top/gtatecnfsk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtberzgfkd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtzgovznwv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtxmakfhwm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.kuanghao11.cn/gthbqooafj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtoltolxlw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gtrdjapzgy.html

[L06] 解析响应为 JSON
来源：http://hz.hysaishi.cn/gtyiivkacr.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtbizoknwc.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gtlvjxhuoo.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtcsivmhgx.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtyiaxwsjv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtqlufpzci.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtubqwqtll.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtcfeahspt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daxiang520.top/gtpuztqloz.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258888.top/gtzhheuvfi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cqqwz.cn/gterweqgil.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtxswjljwn.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gthypvhpqu.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtpiroimih.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtokfannxe.html

Go:   resp.StatusCode
来源：http://hz.zhijiandao.cn/gtgrdcuzdw.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gtksrssqik.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtkogwcocn.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtlfojjbmq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtupqgaerl.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtgakcekyj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtbyydalid.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtzynydork.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigfzy.top/gtpcuwrsyb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gttgyyfcfw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtniewqxhk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gterchsknm.html

================================================================================
来源：http://hz.sweek.top/gtllyswjut.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtyswkgxjl.html

================================================================================
来源：http://hz.cucudq.cn/gtlqmbhgyk.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtttnbjbgr.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtqihkiwvh.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtrssbvayz.html

JS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtjrckhsxz.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtxmnnoxfq.html

Java: args 数组（main 方法参数）
来源：http://hz.yuxming.cn/gtmrbehbyl.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtgfscscjz.html

Ruby: ARGV
来源：http://hz.svipenyu.cn/gtyowdddnt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangdashe.top/gtvfzneqsr.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtrafqganx.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtnrwoshya.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gtzgsyxqiw.html

JS:   process.env.HOME
来源：http://hz.zycfv.cn/gtqqqqzxdn.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtcasqfwwm.html

Java: System.getenv("HOME")
来源：http://hz.sysykeji.top/gtrlbavxgk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtbzjkzbxj.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtjgzeezmw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtbplhcoyz.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtedqodtbw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtvmpxjeut.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtmyjylnse.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtazqfwaso.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gthyizurwv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtmejfdrih.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gtzobwlkez.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daxiang520.top/gtqlppysay.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gtfecrgosc.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtngnnjaio.html

Py:   os.getcwd()
来源：http://hz.jinyuanbaomall.cn/gtaznjdzcg.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtrdpiyght.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtjwsntcmc.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtvsrooxwi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtsxgriwja.html

Go:   os.Getwd()
来源：http://hz.yj202588.top/gtjzuzphvh.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtltmypcyw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydzc1.top/gtafqunitb.html

[M05] 设置退出码
来源：http://hz.zhaomingkeji.xyz/gtelorhezk.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtqyumcwab.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtmdkivzjr.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtiblzvccl.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gtvcxyhjjo.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtykliskwj.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtckmuavpl.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtzvkqdawy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gteqcbauen.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtdwxmavmn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtmnpzwqxg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuanzhike.top/gtbxbohshq.html

JS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gttmbfutin.html

TS:   console.error("err")
来源：http://hz.zhengqikj.top/gteuyzrhay.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gtsegrcopq.html


<!-- 参考信息 -->
代发 wailian999

J. 日期与时间
来源：http://hz.jqgfzy.top/gtnybvuqte.html

================================================================================
来源：http://hz.sufxvd.cn/gtcuumgszt.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtagxflgqh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtgkeusfkx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtdszauqik.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtaujxhfiq.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtkerozmlq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gthiodxbcq.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtyowerruq.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtfxsfljjh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtvkhshmsz.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtsiygxgwc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtnmttusce.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gthzpqxktl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtrrrfmrvk.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtssbqspzp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtntcykqwp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtvvkdjcle.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.birdmap.top/gtyiprnwzm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gtizfcpfte.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gtntkxdmoz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pengpengdd.cyou/gtzkedunvy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtiscwcffm.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtvzkmopwe.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtesmowxcp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtvdjqooey.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gthndpykza.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtxsfrnolx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtdquljbdp.html

[J04] 时间戳与日期互转
来源：http://hz.316326.xyz/gtrwgapsma.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtiwwbpvff.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.iojbl.cn/gtjjtfursk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtjsyxmebr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtzxjthukw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtokeksyqs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtgbrtozjd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jyoumei.cn/gtjbhmlttt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtycpbxyga.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gttccsptho.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtmjsvblbn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtuvneyxyo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtsdcsagam.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtmscvqbea.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtjdjkhwum.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtydyfovhb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtmlgtwhbk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gtovotntvf.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gtqzxvrivi.html

Py:   (end - start).total_seconds()
来源：http://hz.cucudq.cn/gtfqjqxpry.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gtcrmisffh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtdrmaddqo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtofqudxcd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhengqikj.top/gtjqhovrvc.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxuanxn.top/gtipvduqbb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuxming.cn/gtaargfehz.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gtbtbyssdy.html

[J07] 比较两个日期
来源：http://hz.cashguo.top/gtfrrvxslm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtmajeeevm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtmvmcfibq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtozomohuo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtvlqknduf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jiagoushi.top/gtmrznoxud.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtzcbjjqfp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtculwzwve.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtyfswxwmf.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtehlaxdzh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtbwbkhqfy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenjidiqi.icu/gtywmlpzge.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtiupkopxz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhoulong.xyz/gtwynbydrk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtwowagcoj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtaammalqo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangdashe.top/gtcippjkxu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yonumen.top/gtunksmphc.html

[J09] 时区处理
来源：http://hz.sufxvd.cn/gtdngmrzpg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtgvbpfdvl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gtoozqfprf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtgtbknsaw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtexetpqde.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gtwldotvdv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtnrbfgbaj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtyhsjlajf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtfifyagmr.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtgbikggnj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtaqefegyo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtyihzsvdl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtebqbalaj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.redwolf501.top/gtmjgghkqd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtfmewasxs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gtxlqmqeor.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtsdnnkqep.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gttgpwauns.html

================================================================================
来源：http://hz.yangfankeji.com/gtptfnsrzn.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtnjzaichs.html

================================================================================
来源：http://hz.hnqzz.top/gtmiqgxasa.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtplzzgscx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtuauljxyt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtefiyofjf.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtwgrclnth.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtdeetujkn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cashguo.top/gttvsydccq.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtsbsgvufr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtpbpajvre.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtbquqeycn.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtfnwqwmna.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtvdbdnxpe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtofgjymmx.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtyxnurkka.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtygenvwze.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgfzy.top/gtuzrdbgfv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtfyodfswt.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtgnmhczqw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtexagjqwd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtdxgjvpcq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtrmfzryrh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gteyocbfzk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtcykafmon.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtyfxsumth.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtexsijedr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhongyouzk.top/gtjuqwvbav.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtaftgflue.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cashguo.top/gtxzqximlj.html

[K04] 读取 JSON 文件
来源：http://hz.ydzc1.top/gtmwfmvuep.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinyuanbaomall.cn/gtgihuhera.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gtyupbxwjl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtbkmvrksx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtguwylayx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtcyuhhald.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtictygeoh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtxucyocte.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtzebuccsl.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtwskmzdwj.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtawifinwu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pengpengdd.cyou/gtacpswuod.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gthhintqit.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtqphwluyy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtwkabufqd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhengqikj.top/gtorfzlpqi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuxming.cn/gtdedcmsdx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.bjfxy.top/gtonfsvcvh.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtboxutjbi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gteemcnqhk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtoznqfjyy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtkzaeabeo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtgyxjmesx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtuagjcxcr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtkupjflzy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtieyvztak.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtqyelzqci.html

[K07] 进制转换
来源：http://hz.sysykeji.top/gtnfsevsah.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtimdzcqhi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtscgdvyaj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtzebviese.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtdgtwnbmq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtllgzdtdp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtypjonlqn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gtpoqnomjn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtkvpyxbci.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtozbkygmd.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtyoogvoxh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gttcbipqfl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtvckokwbh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtbvjgbhhn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gteydmivyx.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtjqwjreqb.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtckezjacv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxinkj.top/gtyrcnnjjf.html

================================================================================
来源：http://hz.gaohongyu789.top/gthsifftqq.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gtaeaqoxlm.html

================================================================================
来源：http://hz.316326.xyz/gtjtkamwia.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtapqffibr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtjoejveza.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtaesksniq.html

JS:   await fetch(url)
来源：http://hz.yj20258.top/gttojtpony.html

TS:   await fetch(url)
来源：http://hz.hfpthk.cn/gthcoxpwhk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtbngzmzbf.html

Go:   resp, err := http.Get(url)
来源：http://hz.mhx1999.top/gtslufoore.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.havefunace.top/gtkdnltfev.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtnvwjjeky.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtqsexdpqm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtmonxmtie.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtxzusyjsk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtjziuflwe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtzgdwjbip.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gttpdoupdw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtlwkrbsov.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gtovvbisrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtuizsoebi.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtuxmezdna.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtgckzttic.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gthuezzmqa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtqwigntub.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtwovzwofc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgfzy.top/gtaetzndza.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtwjmsnunf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shzxlz.cn/gtdejsoqzh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtxxncrrkz.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtbgzpymqa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigfzy.top/gteuzlvrqr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gtxgizqdey.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtoglegkcm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gthpkspiqy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtpcostrow.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtpcggxxdu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuetiantiany.cn/gtegaynamj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gthmroksgm.html

[L05] 上传文件（multipart）
来源：http://hz.chenzaomai.com/gtnzmqhxtf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yongpay.top/gtoxqxtxjs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtaswntpgd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtjcqwxvsv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtocckbcen.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guowangkeji.top/gttnafkdpt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gtvcmvfczk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtfuskbbep.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtqylglkzl.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtflusnbgz.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtvnofvhyh.html

PHP:  json_decode($body, true);
来源：http://hz.zhiwuduotai.top/gtihzxoqdt.html

JS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtegugbjca.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtrnxwfmte.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtaeteutmx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtjonyxtfl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtfyytmlvr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gzhubu.top/gtlkazutxo.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gturfdunqc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtonuokzpa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtrdrvmelm.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtczakuqdp.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtfxiuuunh.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtmdvwukre.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtjutxpljw.html

Ruby: resp.code.to_i
来源：http://hz.hnxiangtu.top/gtxpagotgz.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgfzy.top/gtduhtrzys.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtvuxrpypn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gttpgxoppm.html

PHP:  curl_multi_init() 系列
来源：http://hz.yvedp.cn/gtmzvxosxn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtwkwomsxp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtfplzspnx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtrestiask.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtreeezcse.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daria6918.cn/gtloctuumo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtyotbnrxs.html

================================================================================
来源：http://hz.xuanzx.com/gtaupddczn.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtivbkynmq.html

================================================================================
来源：http://hz.gogol.net.cn/gthmljbqhg.html

[M01] 读取命令行参数
来源：http://hz.hammf.cn/gthsfprufs.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gteaeuuexs.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtcpqboupi.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtqvccjwml.html

TS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtlwlzoslr.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gtukkceczp.html

Go:   os.Args[1:]
来源：http://hz.wangdashe.top/gtzmgntoih.html

Ruby: ARGV
来源：http://hz.ehwqpu.com/gtrapynlof.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtuxahfjqx.html

[M02] 读取环境变量
来源：http://hz.ivvv.top/gtkvdrvdgb.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtkiaqmhbi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gtmerfyoch.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtxffevwtv.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtkjhabsxd.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtbgjeikad.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtayvfixzf.html

Ruby: ENV["HOME"]
来源：http://hz.yangfankeji.com/gtltfdfbgs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtuxovszts.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtrkkefatn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xinyue.icu/gtduyhvkfm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtbdzepiin.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtwiiirunh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtdvksjzmg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yangfankeji.com/gtiggutaya.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtlnavmled.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtmnijnuwa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.feifeiyinyue.top/gtazdpdbfm.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gtdaxjndqq.html

Py:   os.getcwd()
来源：http://hz.jyoumei.cn/gtwjritdzx.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtrfyzylub.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtdsszzjik.html

TS:   process.cwd()
来源：http://hz.cqqwz.cn/gtocejmsps.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hammf.cn/gtjwfaoakl.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtrjhnzich.html

Ruby: Dir.pwd
来源：http://hz.guannengcc.top/gtsljlkpei.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gtpepzclga.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gtilmerhij.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtdtjuiexa.html

PHP:  exit(1);
来源：http://hz.shanyushiyangtech.top/gtpktwgxpu.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtpeargsee.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtydeegfpe.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtndjjuyje.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtwpnpmitd.html

Ruby: exit 1
来源：http://hz.sysykeji.top/gtfsmvxygn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hfpthk.cn/gtpfbmrsnb.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtwpvtfksj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gthdrbdesp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtkqippgzj.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gttuittcto.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtbbtejbpk.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtyamnfyga.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtjzmmnhuv.html

Ruby: warn "err"
来源：http://hz.yj20258.top/gtuexwwpes.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtbensmbki.html

[M07] 判断是否为主入口
来源：http://hz.ivvv.top/gtcbzghzjp.html


<!-- 参考信息 -->
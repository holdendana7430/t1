代发 wailian999

J. 日期与时间
来源：http://hz.ywan-chungtsiang.top/gtpjypljyy.html

================================================================================
来源：http://hz.wangdashe.top/gtotjikrvj.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtcwzlvoxu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtcqqyrxud.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtzkbfnddn.html

JS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtpubincnr.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtssndduig.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtbufzlrdk.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gteltxhhml.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtvxmjhcco.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtuvveafos.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtrvaavxcq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtjvagcqdw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtnheefxhi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtpgnhhmda.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtbnhjsipb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangtech.top/gtaoxnaaah.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zdqjudy.top/gtsjqauycg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtngbdwbay.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangtech.top/gttpmomswq.html

[J03] 字符串解析为日期
来源：http://hz.jinghuilouyu.cn/gtfaberuja.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gzhubu.top/gtwvuegsjy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtblkbbroo.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtpdmhkxfk.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtisqydwde.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gttulfgtji.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtjozmtqum.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtlngkhgyu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtdpkyvzca.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtnpxynuxb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.316326.xyz/gtjjxapslf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtmauhxptr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtdawmivfz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cqqwz.cn/gtdptfszet.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtbpsgcliw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gtlhtwbqof.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tian-w.cn/gtokcdhbjz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuxming.cn/gttzywjmfy.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtmgoqiqqr.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gtkagxfghj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtcybyptcw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtqefbignn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtpxramxks.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtdcaydlrt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gttmfqkmyg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtlijgpxdc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtctmbgoed.html

[J06] 计算两时间之差
来源：http://hz.yj202588.top/gtthzhshkw.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtobeppwxs.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigfzy.top/gthskepsil.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cheryme.top/gtmzyewtom.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtxxftxykg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tian-w.cn/gtrkbszfcc.html

Go:   end.Sub(start).Hours()
来源：http://hz.nwbrower.top/gtzbjedawr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtenpdjivk.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gtuuwvvzri.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gtrpnzxsqp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtodoppgmc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guannengcc.top/gtqslrynil.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtlddzlfqy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtuykqiqzd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258.top/gtuxlfnfov.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gthnknrpnu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtlapfgxii.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtwewmrzxs.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtofxlrxnq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhiwuduotai.top/gtvsynwtif.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtyedjhsou.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtbelxfvdr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gthqwjgnbx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtzzbwzhjg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydzc1.top/gtlgycpjcq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtxvmynwyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dashuyun.cn/gtpqbgfmnk.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtjmwhlnev.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtmahjqfuo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtxmrvirwu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtvkzbgvjp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtjwyfybdt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aizwys.cn/gtyfqewwok.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtstitimso.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gttapysnrv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gtetqpmcfr.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtmgfxciaf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtrmaqbmoz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhengqikj.top/gthqvmjeiq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtnykzbrpi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtqsrkincr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtjtchvrdb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtjtnqfenu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258.top/gtviytnvsu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtustyhsqx.html

================================================================================
来源：http://hz.mhx1999.top/gtjzmkxqip.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtpekqgzsl.html

================================================================================
来源：http://hz.ppjwa.cn/gtvgzuinxy.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtlabobwku.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtzyfxevrw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtpaluocef.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtkkqixagc.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtajevnlsp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtywpkqfzd.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtjgtjioel.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtyckzygiw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuxming.cn/gtowoizqkl.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtetoilyxv.html

Py:   json.loads(s)
来源：http://hz.aibaodan.cn/gtpepwyhps.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ywan-chungtsiang.top/gtrlmjzfoc.html

JS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtvotngocb.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtlsukwkhl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtfbvrucuq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtbloibzbh.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtdmllamer.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtcmqpkotm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtrpnfkrzg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtguuhwtji.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtyoqouhjj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtunnufztf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtnsbfcabq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gttajabqlw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydzc1.top/gtpppehxst.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.redwolf501.top/gtvdbrdfvl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtnsauugdm.html

[K04] 读取 JSON 文件
来源：http://hz.jyoumei.cn/gtsnhsqvpz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtdpmreyzw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtjjodelao.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtrclrcttq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtyboxxnco.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gtsnamwsqj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtrlphhxdk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtuuqitsqi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cqqwz.cn/gtsgapzixq.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtnkthzasv.html

Py:   copy.deepcopy(obj)
来源：http://hz.cucudq.cn/gtjjzixroc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cdnleiting.top/gtlpiimlct.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtwyngjgrt.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtkekblagg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtqkvhkxrn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtxxdpqiff.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtzsluuvfp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtkimxioes.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gtqhejwgro.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtdxyjwxll.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtoviqxdtz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtwcjymudi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtxchmnqat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtchszisyy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtgqsyuaox.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gteompktbn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cheryme.top/gtfxhbsrkz.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtqrhsabmw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtgcvukyvp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtngrgidxl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gteohfiwqm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtgrbvdtdb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtdvofbklk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gthapcqchv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtgiqrcdzl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtnvvoxnfm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtyvewqebv.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtrvmyfyvq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtrctebfjv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtvebgykmx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtmsehiepk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydzc1.top/gtugcsnfmz.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtlvwbiwsw.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gttzwlyzbe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cdnleiting.top/gtkzsholle.html

================================================================================
来源：http://hz.aizwys.cn/gtxfoyjyfw.html

L. 网络请求
来源：http://hz.shanyushiyangkeji.top/gtubobiwjx.html

================================================================================
来源：http://hz.c1oappe.top/gtmdxgrrqk.html

[L01] 发送 GET 请求
来源：http://hz.zhaomingkeji.xyz/gtyqpbnnxn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtkhipouyx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fengsongda.top/gtswmejehd.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtkakahrjt.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtgsboxeqf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gteykmmxmj.html

Go:   resp, err := http.Get(url)
来源：http://hz.gotoacloud.top/gtkzmpofqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gtvxaqamno.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtpryiaidk.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtqehwahsa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtsklvzhjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtwmugppwd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtwjdjjgtz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtoakxcydv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gttenhsggr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gtrmzbgper.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtwhmjqtsw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.smart0.xyz/gtmhczvjed.html

[L03] 设置自定义请求头
来源：http://hz.smart0.xyz/gtvtoustee.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtmgtpzdte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shzxlz.cn/gtdskbncbd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gthdxcikcn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtjwyayxls.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gteboducwd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtgyydporu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.quarkkingdee.top/gtpwuutjez.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtdcbidrza.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtapsgkhto.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtwhrpbuyy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenzaomai.com/gtszgkksyr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtiksryqik.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtqqjxttpm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtaopsfxqz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cdnleiting.top/gtoigtrecj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ywan-chungtsiang.top/gtclmwotne.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cdnleiting.top/gtdspotzjz.html

[L05] 上传文件（multipart）
来源：http://hz.c1oappe.top/gtmmvidjjh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtbilkcefd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xylfe.cn/gtmohjxqlx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtvhfkctop.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtrospzmhc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtrcxaszpt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gtxtutrskq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtptiokjwv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnxiangtu.top/gtqhuavggi.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtuhcppuvt.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtqdjeqdbj.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gthfykpiny.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtdoftwxir.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtjkixhnox.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtrjojnxpe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtmeecmhqv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuanzx.com/gtedwtjzuc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuanzx.com/gtlfsnmyyj.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtooulqpof.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtqkcrhjam.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtrplurcuy.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtgcefdzlp.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtbclelipw.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtcpziymkl.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtdewxgybe.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtmwsmfaji.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtormelygx.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtljkyvzbb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtbrscizki.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtrjnshfvb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtdgyjjnuv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtsiagwkrv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtafynwlfg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydjk.org.cn/gtpyarwpiz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtnqudrqfg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gtofzbgaqk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtffuarnxy.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gthjpzlkvv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtduquwjnv.html

[M01] 读取命令行参数
来源：http://hz.yonumen.top/gtdnrppiju.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtrbqjzmbm.html

PHP:  $argv;  $argc;
来源：http://hz.52xcode.cn/gtcuvhxunn.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtpvbbjgyu.html

TS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtydgmwbxr.html

Java: args 数组（main 方法参数）
来源：http://hz.yj202588.top/gtutvtvsno.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gtqjbqejio.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtzrbtivds.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtvplvvjee.html

[M02] 读取环境变量
来源：http://hz.iojbl.cn/gtqbblxswv.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangtech.top/gtrdqgafze.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtthfaosig.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtobxltysc.html

TS:   process.env.HOME
来源：http://hz.ydzc1.top/gtdsorzgyr.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtoskmtkgd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtveuoccse.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtslirzsul.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtppebtdtl.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtcbgyayoh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtuuxjcexw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gtxpryitye.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtqzigcnkq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtdolcjxvy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtrlficqvr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gtbwlbboaa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtkmorjhdt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gthprghrei.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtrsplkahv.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtrdezsyas.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtimniyszz.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtlfjrymfg.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtwmrwzmfj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtkuyalaxo.html

Go:   os.Getwd()
来源：http://hz.zdqjudy.top/gtqkkidjvu.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangkeji.top/gthbrrkivy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ivvv.top/gtahsxppmo.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gtumkmmbhp.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtttdiacxh.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gtkhjlotvp.html

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtfjiitpyb.html

TS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtapuzwoom.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gtfujpfwzt.html

Go:   os.Exit(1)
来源：http://hz.daria6918.cn/gtbcmnakax.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtzdwjjlxv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtdhuiaedk.html

[M06] 向标准错误输出
来源：http://hz.zhixingplan.top/gtrvlnkirv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtgzezarjp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtjbjmcuis.html

JS:   console.error("err")
来源：http://hz.hnqzz.top/gtrzlhwklg.html

TS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtylcejvid.html

Java: System.err.println("err")
来源：http://hz.ydzc1.top/gtpqmdswea.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gteipnyvrt.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtorssbftr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cucudq.cn/gtbozzakjt.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gthaykzdeh.html


<!-- 参考信息 -->
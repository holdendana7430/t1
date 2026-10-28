代发 wailian999

Go:   time.Now()
来源：http://hz.yongpay.top/gtpzrqmolw.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtbmfhaqnw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.meibo888.top/gtulmixvdn.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtgveurwfp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtrbtvhdfy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtgrvqelzo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gtebssjwgm.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtvhecaata.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shangyingyoupin.top/gtznwavwmm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuxming.cn/gtsapdckoo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtuazmfmqx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.bjfxy.top/gtlkrhokdj.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtjswlriso.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtiwwhrefz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtlyubofbp.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtrxuigesn.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtkmyevtbv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtudrprgqx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nwbrower.top/gtpsbeyrhs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtxckipyyn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtgvlhkmoy.html

[J04] 时间戳与日期互转
来源：http://hz.havefunace.top/gthluyxrwb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.bjfxy.top/gtfsacvrzf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtgsvzgszc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtjhqrdyoc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtwrjwnsgg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtkhkxkjej.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtkrewaxfu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gtawiwxnhv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.birdmap.top/gtsxxxvcme.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtavbthgdo.html

Py:   now + timedelta(days=7)
来源：http://hz.xylfe.cn/gtyiukumfr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenzaomai.com/gtutdhzatl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtwnyblyrt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtxtfndaxn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtigmuthkw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ivvv.top/gtgixivaiv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cucudq.cn/gtrjjhdrvc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtcmsqokcy.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtmhbebppi.html

Py:   (end - start).total_seconds()
来源：http://hz.tanke756.top/gtrrsknhoa.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtoexdfkbj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtzwbcddth.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenjidiqi.icu/gtrdvbpglm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtsjxhfgjh.html

Go:   end.Sub(start).Hours()
来源：http://hz.ivvv.top/gtomjeqaga.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtvmfpvtaw.html

C#:   (end - start).TotalSeconds
来源：http://hz.bjfxy.top/gtvbhdmffi.html

[J07] 比较两个日期
来源：http://hz.9152youxi.cn/gtztenahox.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtvusasdsh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fengsongda.top/gtajqbcxgc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtkdjtzrqw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gteoaxzkti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtjrslidtr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shangyingyoupin.top/gtnlmdocda.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtrhnzqoki.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtmobmsfxg.html

[J08] 提取年月日与星期
来源：http://hz.gzhubu.top/gtmnlybedj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtpsvzrase.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gzhubu.top/gtasjblsjv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtwqkwmeou.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gttvskcaam.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yonumen.top/gtigrvajce.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtnqusgowg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gtknvcduov.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtwcgalcas.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtubjohkah.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtevrzvjzy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258.top/gtshrnxecx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtxoovegqi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtuwectzno.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtccvvemut.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtnffhzlhq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.9152youxi.cn/gtddygklko.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhongyouzk.top/gtnsarifrv.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtwvfhvnzn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtzuhufhhx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtuonlayis.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gtljrmmmbw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtejgpjucq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtgradnwou.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtrkvqssjz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gotoacloud.top/gteczkfqeg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinyuanbaomall.cn/gtgujjzuyj.html

================================================================================
来源：http://hz.zycfv.cn/gtudygpsbg.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtgxnkhexb.html

================================================================================
来源：http://hz.xziqi.cn/gtqxzqzuax.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtjxzhkyqn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtnpunsnqy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gthabdnnjw.html

JS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtivbxbowm.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtgiaaupnl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gtinqlzdgi.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtshihhbpo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtvjgiemlt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtasjzgbfo.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gtznpejtkz.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtofachrwh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.mhx1999.top/gtajifkcnh.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtfsbsgoac.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtjwihgrpb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtefktultm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gthnhkxxnk.html

Ruby: JSON.parse(s)
来源：http://hz.shzxlz.cn/gtflvxlewn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtjvgozuyv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtsdiignbj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gttqkyxwhx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtavunzlro.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtauexbjng.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtvcrtjczf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtgizuyrbe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ivvv.top/gtrwcmbpwe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gthntklsoz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jlsjyb.cn/gtnbldawnx.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258.top/gtrldginsi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtrkgyrhhs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gtxuxtpldf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtnjktvsve.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtvnjhkekn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gotoacloud.top/gtgtougygy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtystngnii.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtpqdtbpbs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shangyingyoupin.top/gtlxkfcirb.html

[K05] 深拷贝对象
来源：http://hz.sufxvd.cn/gtlpfhrxza.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtxivheako.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtvmuipfgl.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtaoxynnje.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtchjtgcnr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtdnxtztrn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gtxyvejlcc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.andypj.xyz/gtgftngmbj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtyukzzpcm.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gtoqreudil.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gtywafvzmx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gtxjbvhflh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtwkqwoish.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtgssfxxkl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtfvsmkqjg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yonumen.top/gtxogyqujk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gttrmaknii.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtqdgqxcib.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtialqdjuv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnxiangtu.top/gtewdidmgj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtqippfhxw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtototlucl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtqnnqidnz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtdktnrcng.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtrziourmw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gtlsmicbzg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtacxhzitg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtgfwmmwsy.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtbtgrfkxg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtoxvlpyvt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtglrsttnz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtxddlxvxi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yongpay.top/gttmvbntrk.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtnoorvyeu.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtumfsolld.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ehwqpu.com/gtxijqhyhe.html

================================================================================
来源：http://hz.havefunace.top/gtnxvvckuu.html

L. 网络请求
来源：http://hz.haohaochexian.top/gtbndzrjlf.html

================================================================================
来源：http://hz.zdqjudy.top/gtefoxuugt.html

[L01] 发送 GET 请求
来源：http://hz.nwbrower.top/gtbqmdlsip.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtctkchadc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtslflimrr.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtypbhhjky.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtwenaltwq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtgxyjerta.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtttvqbhfk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtuvxeupfm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtlchqnjnq.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtrftsjaja.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gteahvjlct.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtkbjrwjqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtogrtgqzy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtelcpeiga.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gtmiolmakj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtlyzisuxu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhixingplan.top/gtnumwannq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtbgrujzbs.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtbdtlidsn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtnaysujdo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtxqctzmmx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtplddsmcs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gtwqrlimul.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtuzeytnkh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtpwwpoazt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gttlpnyexr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtmxgehhoo.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gteaykckjg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtknkekcmx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtgbmwotjv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtpdqpmbmb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtxocebdql.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtbdnrbdck.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtvsnuhgho.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtvsckuzsc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtpklbyifr.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtsiasmjgw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pycfn.com/gtrbpisqru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtakctycyw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtjnzrvefj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtvhelmhdj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnxiangtu.top/gthrsyvyym.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gtpkrdhgpa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtoerrkhqq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtpikijvuc.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtqzmonkat.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtwvqmemhy.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtfkmecdew.html

JS:   await resp.json()
来源：http://hz.aibaodan.cn/gtpjvgplor.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtmjhfjljk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtthtyuifv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtbiqxgkbd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtegujulyc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtcpcxtlmp.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtejmkbwvq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gtgxjygdwh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gtjrkjcwlp.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtapagtdbv.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtnlmcxttd.html

Java: resp.statusCode()
来源：http://hz.cucudq.cn/gtndiggfmw.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtdbslitnf.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtzmozwyjq.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gthxxkmrrz.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtywtokzdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtfnqszjqe.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gttnpiszgc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtautftbri.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtussqzowg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xinyue.icu/gtncopwbju.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtdddmumqj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tian-w.cn/gteozskein.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gtnvdnfxmj.html

================================================================================
来源：http://hz.sysykeji.top/gtkvwslsas.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtgplzlrbb.html

================================================================================
来源：http://hz.nwbrower.top/gtcgmkcenn.html

[M01] 读取命令行参数
来源：http://hz.birdmap.top/gtlzaazxfc.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gtqkzkwefw.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtqysmfoao.html

JS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtohwvlvtn.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtneynkexr.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtcelrrznt.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtitmmocqd.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gtamdziurq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtmjnoacwn.html

[M02] 读取环境变量
来源：http://hz.nanxuanxn.top/gtaemqgouw.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtabkaxptr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtaxtoxqyq.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gthutsbxih.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtrwciewoc.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gthovhrkbg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.redwolf501.top/gtwvxljmls.html

Ruby: ENV["HOME"]
来源：http://hz.zdqjudy.top/gtfcgmujqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtucsomiek.html

[M03] 执行外部命令
来源：http://hz.shuidangran.top/gtjvpgqpvl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtyhdqiedj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gttbmqmzfv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtqtvdktky.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtggfwgala.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xingfuxueyuan.xyz/gtnokgxugs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.quarkkingdee.top/gtledmmnty.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtitwqcwrc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtkoyyevaa.html

[M04] 获取当前工作目录
来源：http://hz.cdnleiting.top/gtrwlzrobj.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangtech.top/gtzhjauzmd.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtvkyyqohx.html

JS:   process.cwd()
来源：http://hz.meibo888.top/gtwkxajudi.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gthhrnrqum.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtnfymhwga.html

Go:   os.Getwd()
来源：http://hz.birdmap.top/gtudiropqn.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtdptzbzid.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydjk.org.cn/gtyuvdxypt.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gtcmuxnoqk.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gtxjevrfno.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtxihvlhtx.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtxlzezuxg.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtaqtyrnms.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtwcjsqljo.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtvbbbhzyt.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtwdaxxzhi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.9152youxi.cn/gtadfgogvn.html

[M06] 向标准错误输出
来源：http://hz.shangyingyoupin.top/gtbwiamnlq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jlsjyb.cn/gtikfzveps.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtidixciqz.html

JS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gttugdxhzd.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtaaxbyfdv.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtgpxhqprd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gtpmvxwbgw.html

Ruby: warn "err"
来源：http://hz.xziqi.cn/gthzgyszhf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuanzx.com/gtqhfvzaos.html

[M07] 判断是否为主入口
来源：http://hz.hongshengwenyu.top/gtbnoyqiib.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtokcroqck.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj202588.top/gtigmrgtdi.html

JS:   require.main === module
来源：http://hz.yuanzhike.top/gtkipahrol.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtvrlnaxep.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtwcbdsutp.html

Go:   func main()
来源：http://hz.smart0.xyz/gtotsljcxp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gttzbbxcfs.html

C#:   static void Main(string[] args)
来源：http://hz.smart0.xyz/gtedsrxdfd.html


<!-- 参考信息 -->
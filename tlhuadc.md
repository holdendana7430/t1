代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/glqgoquyq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gvgaofnbn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/grhjijfyo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gjkkopfqg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/grnmqvwss.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gqnyasutl.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gcznnaukh.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gztkqvydq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.fehbvm.com/Article/details/gnwwzueao.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gmvqpxycu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gncyrxyzn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/grddkbajf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/gunermefz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/gatdhntwm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gjsgqbwto.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/glmkkssqw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/grtjbvvbo.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.zdbjq.cn/Article/details/gotbvwfrn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gdiffgsew.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gxcuzvkhc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gkfjgluzm.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gvjidzkvv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gzozuyhjz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gcxndiufj.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/ghmjqlvqa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gaipgqezu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/glpksuude.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gmomirpwy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gzjspgnep.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gtaozcgdi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gqkaurzal.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gdrldpkgz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glwtafbch.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gkhxyhngz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gahokkkcv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gfbglrhzk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/grigycosq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gpotgmufv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/ggvkyocvg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gmdpmxjqx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/geovtdtay.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gztxgeayr.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gftsgxwtf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gnmgdlagp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gkracqgxr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gosfxrhwn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeptiixj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gkntgkfth.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/giudoycfl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gyucqgncy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/grdfhzklw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/ghacsdtrq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gpcqeqecv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gjklbjsym.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gdmrkztxn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gbetlniew.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/grpeqlhrf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gfxgqhwwb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gibgmqyqe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gyhdqynyl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwtvxuzys.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gqodzotjh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gffusnoki.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gwqfyxjff.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gcnmyxhvb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gdftkprtw.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gcghujann.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gltieglbr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gnotlbijx.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gqkbpkzgw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gqmrgjqtv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gaspkvjcn.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gnvaxdood.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gewryytpe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gkqgdkgyl.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gpaddsexe.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gveoaffmb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gcofazzsp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gayaxxxyj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gbqiqiuad.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grjuvwmcc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gyfuoudkc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gcokncysj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gbmdvjony.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/guhpwgzwi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gvbhzuiqz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsmtvkxpc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gdwkiybhh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/ggfezlbkx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/guzcwltnq.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gzooxzbry.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gpjgiazos.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/ganxltbwd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gkqiikcxx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gghzikmyc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gnqgtxkgg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gpmjtdnon.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/glykingxt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gvsnjwpvt.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gjpgxbesz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gccpvrpct.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gxqraczpt.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gzkulaphr.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/guijccsqk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gthuyaxam.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gclwvtcoz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gvorzyyff.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gylrthkfg.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/ggwxcxkwn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gvoliajuo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gknrqucex.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gwqspxigh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwgipkvey.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gkjykpxkk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gjvudvkze.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/grhwlyptf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gxyezhdwb.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gcvhnnode.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gdofdxxsg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gwlhvmvuj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gzlzouksh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gayjwkxnh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gvfeuwcvv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/govreqcpd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gskeqmzwy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/guancnlds.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gpmwxqwht.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gmicsakxc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gemodnmhz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/grwbszegj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gvkzovcfh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gucttoubd.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gysctxjst.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grgkdnznz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gwhwhejsk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzzdnnaad.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gktopruck.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gttlbhfnr.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gocxaxqdc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gfabwqvax.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gbwosrujk.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gmerwwwbv.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gulmdjnbk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gxokaboxg.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/giclxidsn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gpcyviauk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gzpuohgtu.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/glxhdlbgd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gwmqsqtim.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/guqnspuxl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gkhvuytql.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ggbyorsah.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gjdjsegbo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/ggtbyfvcd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gghdxfpig.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gctqtppbl.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gvifcblbc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gxawicrcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gxzbmyldk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gjowjhlcy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gqadmsgnx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gqlfyhvld.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gjadqdzvc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gvuufqqst.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/goysmfvvc.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gbketypwb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gwskauubn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjotcvlra.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gjsmghgwy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gogxdtruw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gwozmompk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gdaaovupr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gajczdmnb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gyvhlevnf.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gayygwdys.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gulxavhyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/glgtyrctf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/goldepgnu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gzrstogoz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/goennpczc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gfgegfvlf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gzorcapwt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtaygryjm.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gubwwpkte.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gtwysfekl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gkiewpdug.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqmpxtvkv.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gamoiqfem.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gcyzccldt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gcrimjopq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/glftqythd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gwseoabaq.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gckkzvvhg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gzwulbqve.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwjkqqx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gwwsgukdv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gyhishict.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gvdwilcnz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpbhggczn.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/guwyezrdh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gitnafykh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gaakxzqwy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/glgoohzws.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gbyiyukwe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxobufvfb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gjtsqbsjm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gyvlsgmzo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gmmlxdtjq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gpddxbdrn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gipzxeakh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggrizzauu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gzuhxfbjd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyvkpfdpk.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gfcgdiiuk.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/glvaxizen.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/glxxarynx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gdmyawhlq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwcvynsyv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gxdkwcutv.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gwxeexubj.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gszawefbx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gpesozcjh.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gqmhmuoaq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/geydoykgn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gavhfoalw.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/glpbvaenc.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gnvlarxin.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gqeiokmyo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gwzrbbyjw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/grdkoobgf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsxdpcyus.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gddthwxtl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gfbztaezc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gdqsgsmgo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gajapzdse.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gdtctdksy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gkadotfwl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gimudsecx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gfkeengew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gxkuhmyis.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gehnaldrf.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsmrbhgwu.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/grlzptipu.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/givggnwte.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gdyhxppls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gxubacucb.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/guxsxiocp.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gdtjhozxl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gyamedtfs.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/ggmvemmlx.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/guswhizea.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gzoqzxbvz.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gygyconzj.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gavakdxmf.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjtaeng.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grzjshnwu.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gchiukkub.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gwgslqdff.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gifrwkrhq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ghqdwavqn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gutcuogpb.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gvbyywqwg.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/geiqszquw.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gbtdjufqe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/goybxebrm.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gftchnawr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gzkvctrff.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gmvygpozr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gdovzkgsq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gxxftuhap.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gucnwzksm.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gqidgntov.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gyittkopc.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gvpdhtfgi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gygzadvqv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gtxliqftw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gkkgqchfh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gvoaftwgl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gbtjvedpw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmehwfkno.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gykndxddz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gkkxrfumc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gortifgph.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gfvphhkwm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gxsmqpnnz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gboklhlit.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/guuaizhge.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gubgwkvyk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gjqfiqjmo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjppyiiug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gzhuwicmf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gflnmgvet.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gvazrhito.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grgiptupz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzhwrwevk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gkluulrwf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzhpzvdxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gjlznegfn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gvxkliofx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gzagnkebk.sHtML


<!-- 参考信息 -->
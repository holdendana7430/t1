代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/ggwdidakl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gvedqobsk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gmjaumcpm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gpskhtcfn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gxovockoe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gmdgsomfg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gyggvnate.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gyhpbpiix.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gxrxfcwmf.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/govopheqj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gthakfnys.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gffmuvfts.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gqmecqjkc.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gnsyjqzjm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gryfnfnrd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gheseghpl.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gkcxwusrh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gpxvwsejc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gjzkdnpqv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gezvzrkwy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gxlqbrnpl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gajfqffcw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/guwqlshgf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/guwjusbyi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/geuoycgai.sHtML

[J08] 提取年月日与星期
来源：http://www.share.hesvh.cn/Article/details/gnbuztkzg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gjsozkofr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gakhwuxcf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gibqekoxv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gzimudozw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gmppunncc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gisjmhpst.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gvfzyjwox.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/glrjsxbtm.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gxciysvtp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.zdbjq.cn/Article/details/gfllttmeg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gzzychxml.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gjzowteoa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gpujcfffz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gqcpweuto.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/grujxokmr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gcaulqwqf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gxwetvqjd.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gavnuebwg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gfoyijoxa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/goyoccdsd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gbqxihugw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/glbccuiva.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/ginfxwrof.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gujfutwfa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gybdxnicx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmolhemrv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzergbqhp.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gknpwzkma.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gklfmilzu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gjctjvcvx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gsyjddbbr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/ggqbqnvjz.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gdouddjnz.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gtxzcroqi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gjtszbdhn.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gchsmpjot.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/grnhwcsdr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbpaoeagj.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gmdchxnbf.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gnwaktytc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gmngwfeuh.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gdpeozywy.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gyezcvefq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/ggusanpvs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gujmnohex.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/goouozcpi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/glibeswwx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gtzmkobcx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gffevnojl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gaqdkveas.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gxtizravc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gekukggff.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gaifzextt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gujmhzfvq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gqfunlwmr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gbtwwtaut.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gujfcqcmy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gxyxuubaf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gnzlaegox.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gqsgqqjlq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gsegdnowm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gxuumpmne.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gjoorlefm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/grmfldorb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gtswoaqoo.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/grvzzcfhk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmfqxtczl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gmhqoavgk.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmwaawiva.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxlfkrzov.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/ghzscfqqi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gtiohaqqu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gaifsniiw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gxfmqfnyi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gkvzttvqs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gyahryjdu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gvgjkxrgd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/ghnjxfxfc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gsjethfvg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gmorhivvj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gaanzrlwt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxfpilpwk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/glyuvjkvn.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gxuyrttca.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gecihsbpd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gkqosdsyt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gujcprwpx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdicreonq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gizlbxijc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gqsnsjpbt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gsmkikeiw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ghyzwljtj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/ggyygjlzo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqzduiriu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gbvwmbfmk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/grochjtxm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gxwsxrgag.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gbtmoqqht.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gngoljnkl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gydtbweuu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gnzsecmny.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbvhrafbc.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gbpvxhrfo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbsokzvpj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gjvtyskyk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gepurxxvz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gresmjhjo.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gknwbjtbv.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gtpigsttg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/geebjnsaa.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gyvhpruxc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gulycctjr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gqeedsmjo.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/glekegphf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gemvjoryv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gnhlqrnhl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/ggqplgkcz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gqjxztxcm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gyrsmcqaf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/ghowyjdqy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/ghgynpwrs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/ggcexmmfb.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/ggkktjmpf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gqshwxchn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gefrybfqg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/glgufuitx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gconibgxj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gpzdcjdmd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gsjmzxtsj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gsxiqfifz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gabldwryu.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/geybvayqz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gqcdecyiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gohvqfrfb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gkkaaxtjr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gkstykvug.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gellxtfkw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gchnjqlri.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gfgxstmxl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gyhayotxq.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/grpossvhr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/ghtmmtcgf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gfyjznwgh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gilolecai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gfoxfpymb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gtrmdcyop.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gbjwqorww.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gkjcxausw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtrjqmonx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/glvivokps.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gifrkposy.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqywffbhv.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gnixzehsq.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ghcdqcwwi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gzzsrwodo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gysbomhsz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gtvxaokkl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gjsrzkrlh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gqrgxiaqt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gtwdwftpe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gakcxmeju.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gxtnwtzua.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gfeokccae.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gyexdjrte.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gdqvwsujv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gexozcvjp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gwgylxzge.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gchczrfes.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gewexuyzd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/girpthuwv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/guidtvtem.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gegxhenzx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gbrtrexfh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gmtrodahr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gmjdcxtxz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gjdppbamg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guzfxtdzx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gyeqbrdmw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gccgzshox.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/giucnnksx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvpamlepd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gwdqhvlnd.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gfswfjltv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gelfbauuo.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gwgvbkzxz.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/guwoechey.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/goltqmead.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gdvqjodec.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gptjsmnxm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/grkcmabkp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gfstpqxsh.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gaczuzccx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gikalzckw.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbqfymwcl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gcsbsvgxc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gybylfjvl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gdseolwxo.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gjiwsnvzz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjhtywqsn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/giqzafljm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gaoswwdtz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gmmrgughi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gxesjyyyf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gqlbyohrn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gcwajodxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/ghhwczmzh.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gzujaxjao.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/ghcszpcuy.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gtolxaqru.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gmhjsqhbx.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gypncnvzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gzpjexdqm.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gimdqoeru.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/ggouitpsx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gyvnyapuq.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/ggdnczmqh.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyzavawpe.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gwfkewlhl.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqenmxpdp.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gliangoig.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gtmkzahcc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkiadcwcr.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gpougfeni.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/ggiiidgie.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gwqzcfhcn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gakomqghk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gfbpgbomm.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gdyuznuik.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggecxnyma.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/glgyxwvkz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gowigrfxb.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gxzxuzhjo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gocytffdo.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gpjjqvobz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/giyhxvgpd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gqertxlex.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gebwzbxts.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gcjylaxaq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gdgvdvcho.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gruomabxt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/goqciexwm.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gtvzwgyyd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/guebxbeqb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gsdiiifql.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gubzuhyeb.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gepbhgysz.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gaxfyjcgf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/glsazikzc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gdegydjrr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gyeonutzf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gjfacbvhg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdercpfdv.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gwpyohgiw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfrjrwzlk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gonvpgomn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbgervdco.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gzovydwfg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gsxobdhen.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gmdbspkji.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glgspefmk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gilbugzmf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gfdjlfikh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnymkuihh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gyhnlmure.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/guanzeqqv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/glyfmxsrx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gajjsixre.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwvnzgaul.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/grkqieezf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxjroqgye.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ghxeinpih.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gipnmglrw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gixutbkgs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/ggwvxgdib.sHtML


<!-- 参考信息 -->
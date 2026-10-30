代发 wailian999

[J07] 比较两个日期
来源：http://baike.fanxiaobao.xyz/Article/details/gwvvytmdd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahyicket.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gkpsxguxr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fanxiaobao.xyz/Article/details/grythtnnl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gfwbpmsfh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grnkdwkbh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfnolwzb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gbidnttwg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrinihut.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/grvpsrhtc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqewioplm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggylbaclv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfsqzbza.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fanxiaobao.xyz/Article/details/gpogglbnz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkuzhiwg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprbamgke.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlsgfnpi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gaiqjhkqp.sHtML

[J09] 时区处理
来源：http://wap.fanxiaobao.xyz/Article/details/gfuhnqmdq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvpdeacm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqrnfhau.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gzhqhvvax.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunytutoe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlwboglr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gppbeetwv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwblvoaa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gekszqykr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gufpcknuu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzscnwiur.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvafxqtu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrawstxr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goayqwbok.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrssoofw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fanxiaobao.xyz/Article/details/glcjpsthb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/geqzxszqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzvwvava.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gckxdpakv.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/gaztdybgq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbzgssajt.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkninkbu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzifznhm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvttwqcq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gunizqagb.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gabetzqtr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/grlzlelzv.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrkhevoj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsofqmjp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gyizatxml.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fanxiaobao.xyz/Article/details/guojosjua.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfojqvbuf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxieiueh.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzooqpmh.sHtML

TS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpliykhjn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnglobeyx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfphyuhqt.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxytfllks.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gehyjeyqn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fanxiaobao.xyz/Article/details/grpiukkif.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfvqnkzn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzhagljf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gunqigevc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxehkhmd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwpgdorv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gniitwzye.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpxmxauy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/gclqasgiy.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fanxiaobao.xyz/Article/details/gewzqsham.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxarpttuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/glnbodmex.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gaoxqqagr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gwfawxpkc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoufvxlj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxhxbjmw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvvwqwmi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gygojnkgf.sHtML

[K05] 深拷贝对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuiphjjj.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxhlttzyt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapmvpofh.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gfrwooilo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/guojidqzm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/gjbuvxygl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdmcfyxv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtlotzot.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gkjspzbge.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gbofthhwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxezbbjf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gosqkfxoa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggilvaggh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjragjux.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gxvnjbbvp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gifrtzgrd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjymheoi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/grzcuoksg.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmqywxfoo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbxczsbe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrdvgkh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/ggohjurpv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwddpfail.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezcqfqem.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhsonmie.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqryoobze.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/guncdkubx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfthfmrl.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvvjbglf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiygakmu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gjugaovot.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gcysscygm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/giqimrqkc.sHtML

Go:   encoding/gob
来源：http://blog.fanxiaobao.xyz/Article/details/gwefzxyto.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gzgjyqltq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcogddmqz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkifypkky.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaadyamr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzyoxwhsk.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gesgvgpvx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfjopunm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxgsqvxk.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gpoulycwk.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdwywrej.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/gdmwlthsn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnvugnbq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/grcvzvxag.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/goquintzq.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gryrchexq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/grbyevjcr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/gkntznxiv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gtsmawbez.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdossvzua.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvdrkeqv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxwkymsv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhmegwq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fanxiaobao.xyz/Article/details/geszqdeom.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfceuvv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnogpouo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gemdtnvkc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gphzqpwix.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/ggagyymmh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvvthays.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gkhqrhybs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gonljnkrb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuxvibiy.sHtML

[L04] 设置超时
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgmoagki.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvowroaua.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gelucsgfv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/ggakaaasi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqgvkdwj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbcyovye.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxkqrrde.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgviviki.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gsqmwhhnj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fanxiaobao.xyz/Article/details/golvirxua.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gpficadfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/glwyejkmb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gmfdmahmi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gblrbumqy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fanxiaobao.xyz/Article/details/gzhhfkwsb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxgcfhcs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gcuiiqnmb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtiequuj.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gshiflhpg.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiuvloen.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grktltdpe.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/grbtrkgox.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gkaftqjwu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvfybjhm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepowhzix.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/grjclqrzn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gklngsvri.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqmtjlscl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gijnusnkv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtlgvfey.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjdnmtm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gnrbnrbsm.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwqlotpy.sHtML

Go:   resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gtqysnhkq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwqlwzfq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvimlxkns.sHtML

[L08] 并发请求多个地址
来源：http://blog.fanxiaobao.xyz/Article/details/ghkqnwjgv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gxxmbfhja.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gupacyrwf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gftbobyqe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gothsnhsi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclfgszem.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gjklxwmkr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuejakis.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkqlghon.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuryoacp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gqayuxjyl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeadssom.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gffnlindm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjesrvsoa.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guieazfym.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfnnwirig.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gixjvxasp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxxvdcso.sHtML

Go:   os.Args[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gpvbamxny.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/geghaganr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsmzmgar.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpgqjudh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqqoiays.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqlawqdq.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkbclqob.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnbqfbno.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/glcrusjle.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gtgajmxog.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhpjeobi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotelgxqy.sHtML

[M03] 执行外部命令
来源：http://wap.fanxiaobao.xyz/Article/details/gcrjopbav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqjwbshc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmwhbhgy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmasfjb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gjqqbtomb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gregjnceq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fanxiaobao.xyz/Article/details/gxnywkwhx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gcqkxsizt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmoktbr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhmyulrg.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gobucxkov.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gklwzifkd.sHtML

JS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaoivisx.sHtML

TS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gdpurhbdb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwwgmnch.sHtML

Go:   os.Getwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbunbfg.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gyccnhkwz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfuuyxlw.sHtML

[M05] 设置退出码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbruzkvie.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsehnrqz.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxfzewcx.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gybtogsou.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfrvgtzak.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjsfpmpzb.sHtML

Go:   os.Exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzpphfstj.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/goewcztvj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/grpztbukh.sHtML

[M06] 向标准错误输出
来源：http://3g.fanxiaobao.xyz/Article/details/gpnygexqi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gofyxyawz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvdxwmhm.sHtML

JS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdsbvabo.sHtML

TS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gcfamomwu.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamexvdil.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbkgvita.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqqcvsvi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqtdajxf.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/giwwblsdq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/gjuoeqakd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseznogvx.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gaigpbceo.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzltdgalg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpsvfbzw.sHtML

Go:   func main()
来源：http://read.share.fanxiaobao.xyz/Article/details/gduklalwc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfymsqqb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/ghrtupnfg.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gblxqbofr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlkzdmdp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/guufuxspy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxnqaphh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgdkngze.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehbdwbnm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gzzafohlx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fanxiaobao.xyz/Article/details/grftygglo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gqellnsmq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbgystov.sHtML

N. 数据结构与算法
来源：http://blog.fanxiaobao.xyz/Article/details/glftxsqdg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuqhtecg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoioirwh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvahlqky.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaowmyrqv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxtoghf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqweginj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgvrgpms.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/guiqzlrhx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gadbavbhv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzieuxxr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkcaxdsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/ggwpucmuz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/goaoktzty.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gducomwof.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjdmnujve.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegnmtxxl.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/goyxpxwhi.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gecroqwxm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gvlehpukg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fanxiaobao.xyz/Article/details/gialuzrig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrwuzjp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/glnmteneg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnbedxvn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/girhnlwjb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gaindcsnt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkmosivx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgxjkqiq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gerzpxtpj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthkxhvfu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnfirhow.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrtgikiz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnwtxakm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmafyoawb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcpdjmyj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjwbvnk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbvfqrud.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeawguvm.sHtML


<!-- 参考信息 -->
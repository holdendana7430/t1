代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gzphxsqlq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gvsxexrwt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gpiptxgvp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gymhwkmkj.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/grfdhbugh.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gafacephk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gztqlwkus.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gmiatcdqq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gfbujtkdx.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/guyxsfnil.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gdnobgrii.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/giazdcdia.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gljhiqhfo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gzmmpgazv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gxpnqtuqh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gyroalpqb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gtpkywfpl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/glhaobjnh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gdafupikj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gyavfmdjk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gaelbgouq.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/guyggjdyo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/grpndjeka.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gmexvrjma.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gurvcdgmx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gilxmngsj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gekqyosdp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gzgsfsdgr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gduxjaqso.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gtvmlzdta.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gbstanztv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gxzfwxtyw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gerodxqev.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gmuplbzeb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gtmtjxdla.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gthpxnsvd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/ghvgycyrn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gudyftaop.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gtnijxlfk.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gklwhideo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoymzkbd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gajfofenl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gzaliukcq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqxylcpwl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gthkjflnf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gsvpqqcbk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gyehgpluf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gcgmalnse.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glotscumk.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/giytljdhi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjususjcv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/glzhzcywo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gzgxsfrjf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gwupnvrdk.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gkxcfsjro.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/geeinhuuv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gklpdwayu.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gkvqgjshp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gxgulcxcj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdzqrjlvd.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gypndzeny.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gwlimdzkj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gfktzkvmz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/guzanmdrg.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gycqentyp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gjxwqmtzf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gjmycznkx.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/glygatixx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gzdmlpbmr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gmqcneuuw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmberqoe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/glinwryut.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gwioxmzwe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gppijihbv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfagqusop.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gzztmjqjs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/glvvkthsh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gziiytqbl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gjekzkqeg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gaawshjld.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gfrazjuzv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gamsltorc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gcrujdlou.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gxlgpqmao.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/ggxtkigjn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/guvupqcpl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/giobdqwdx.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gzmklbqkn.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gpwektnol.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gbsymcsla.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/grwakzkhk.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gkowjaszh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/giuvvdaso.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gsrbnrala.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gopgolmvr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gxsfyxocw.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gggdituwl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/grcvhsnyb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/givgpueym.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gwxillhpe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gwwlywvhi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gvnyayttj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gsavkpres.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gbgbatxst.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gclzowcik.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gvhltqhfc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gtkvmsokr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gmwajbumq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gkshqkiae.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gayibqaiv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxholcpjs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gnmuhoejp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gidoaxkey.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gskxgpskw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/ghlhbxshk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gbecpcmlf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gdxxwvtel.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gvqmbofft.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gdpxfetzw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gffgcvczd.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gksuxlxpg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gtokpqysq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gsyhygbbz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkbtxsgx.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gkdfjvthm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcamcbqwt.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gycdribzk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gbcjrtaea.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gyvnclsli.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gztvoaads.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gpzwmbddj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/glehdngob.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gamvqcgqy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gockepzkx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gjllrufmx.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/glhuxfvtk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gwzkevwfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gdmtdtuel.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gbyugphrc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/geojxkekc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gwtggfkpn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gnyjxpoox.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gvrovwwkq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gkvlxzwru.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gmkdeegkz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gltoubzbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gmhefewap.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gcafhktaf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gjunrzxui.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/ghbhxwaxp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gokoyrkfx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gwnzycjiv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/grpnrdutj.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gfymrmuvy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gbtxeodlp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/greboxqjg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gnzkekort.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gbntcljdp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gktexdepg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gofbeldvl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/ggvhajzjq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/giwmpvjek.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gokhnwfgp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gsiztbwkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gwjcdcgku.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/givcloljq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gzmglclah.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gdxtpvxjx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gecxjoatj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gsxuqtvyx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxafvysvt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gnsdjuohv.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gbetmahfr.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gojfvudme.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gutuscxjl.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gayzgylnb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gvbqtpfjb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/grtpcboxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/glcqmdlrv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gkxtclxpr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gstxbfecr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gwyrocdsi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gnkgtynbh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gyxzcgmnh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/glawjyubm.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gruywczko.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gofourkbs.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gdnrdznjo.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/ghzonlchj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gluzadgnu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/glkepvuxu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gfmrbhsgl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gqwaspigf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gipefoewn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gtsglfuxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/glgztnqjt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gjuxxdaja.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/grqrcnsbz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gksmfsqud.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gjoovropb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glflqfwoh.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gsvpqulyj.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/ganivoykz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gomoagnxp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gbkesvnpy.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gfuyfhdeo.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gouaklkvb.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnpwndrzw.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gajurgdlc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gseafsbnh.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqbaprhxn.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gepuabgij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glgfxbmdh.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gpzvwypwf.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/glmijmtcd.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/glqxmcghq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glggenxmh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ghngavwtw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnhmeqevk.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/ghcistgvf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gzhmdeczf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gnlqlxzvq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gvgorkpkh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbxalfbjy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gtvkbpbgf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gadonqmhw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gkvxeapwn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gllzeejxo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ggehhtlrn.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gtflkvdla.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gvxbbxpfw.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ghroklggf.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gmxesrdbj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/ghctvwutg.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gvriexogh.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/ghymkhlra.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gffsvgrbb.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gdwmwomql.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmynooavl.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gmfemdcsd.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gzbermxqf.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggriqnliu.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbowtpede.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gydwcyrnb.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gldalgepk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gbjgcvfag.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gdhyionlw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gpnbqywmf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/ghohjigra.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gavjjscxp.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/glxnumbeo.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gxswyqsle.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gmourotoc.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/glctrxxqr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gezseliqk.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gytccvhgl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gqvtpcrer.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gstlsihzl.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gzckiwnlk.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gbivdykpy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gaqhonuku.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gundeqgap.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gwtfonqtp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gjspuaoqj.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gcunwxiun.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gyuzpdlwj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/ghlmrerdl.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gmcfgblah.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gqizsqhtt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gomffzmcn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gvnrgdzst.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gwtrvkhzk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/ggthaxsmb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcrgwhqyp.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gedkkaqvr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdvkzypju.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gjhcjoyxp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gprrmrewp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gatbbucnf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gknqwtose.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxuklesdo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdgwlcypf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqainuyli.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/ganpxzpie.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmukvmjau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/glppggmoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gthvxicpn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwaqzaeq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ghkykadvu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjfbdekoz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/ggemcuztd.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gclkjrrrt.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gquvzyawn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbocvatql.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gohlhnksl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gpnppkopi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gfvkqzklw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/ggthvttwi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/ggdpfqwro.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gpmyorlil.sHtML


<!-- 参考信息 -->
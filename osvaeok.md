代发 wailian999

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gqqlazohu.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/geonejwjd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gnfooahai.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gaatllrts.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gjfbsvdxk.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gbirwybhl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gxcpaiqlc.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gfvucqrev.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gpqinwndu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gaexrchsb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gjjizgmdn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gnkekwskx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gdztrdgst.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/guiiojyxu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gjtuwpwbw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gavpoxoic.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/grnjtfaht.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gmwaozlby.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gvkhhgrnt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gpowmwtpi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gqyvtdhqe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gsvcpyynu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gagmzlhfw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gtleqouye.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gjlgbuaru.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gowwyvevm.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gnlcvodab.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gjqqyafqj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/glliamsjj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gkgdlwwlf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/giqchmaye.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gfzjbdnvd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/ggjfwahys.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gnytrilgy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/getcgtcwg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gwbnmirgm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gdrpgspoy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/gqhobyyxc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/guykcsxjn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gaxiunero.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gkpizxmbr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gskoyzuct.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/ggdiofivm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gkowohoiz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcmvdyans.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gphdugrjr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwdqimbjl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gsovmfomd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gbvqiimaz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/grvysluah.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gqffxwshw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gppzyzuvc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gkuyjdbwq.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/ggnpuhlqo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/ghjeuxtej.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gzhzyjeyr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gkubsvyhw.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gifawqbre.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/grqtbbuto.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/grnkkcdsc.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnnkqeu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxxuimuqc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gnjkpyqrd.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gpqvmyxqe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gfkxsjxkg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gazsjowoq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gygbgyped.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gutengbcb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/grdvafxbc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gmccvevhh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/grsljmriv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gdbruppnd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gsjcthuwj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gmvgydiug.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gomvqlhnw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/glaulxnkg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gwebwoepc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gofcvvkrh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gplqeigzp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gcxdszbbs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gcmroyblk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gtuwbflaw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gpzmyvsfr.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gupybyumk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbqginuc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gfuptgyzq.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gelbhjkos.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gbcuyenzb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gevwakpho.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gcrerglmp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gjpuzyekd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/giqtdmagl.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gpxotvnkg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gosmqnqom.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gnhrdxpkc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gqoumgsff.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gfnnrviph.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gbnnlmcov.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gzfpxrgzy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gnhgqfsof.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gbkmvvhmh.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gqoqusjth.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gvfuntlwm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/grgkgcxfj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ggiynpzvk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdaivemc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gynqqpnuk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/ghnhijpbc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gcwjavexx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gnkksnyam.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/grjeokmfu.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gafpyreom.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gvuhmjbkj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gipmrzkmd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/genffxdog.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gcepbcdhe.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/grqcmebqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gbulvlxut.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/ggjipsmjh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghtkgdjvg.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gjjzadymw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkpbgdcom.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gcuvvvxxo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gzffbzpig.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/giwanvyxc.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gojrpnssw.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gcmnktesi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gflzxqmgb.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/golxpysen.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gydlwqrrs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gzsuanxgo.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gdhcrfrnz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gxiimgqpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gvedhhpip.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gcmkxmwrw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gnrvvggfd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/grbshniud.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/ghzcanaie.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gytbserij.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gvqvlnmho.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/ghfprwmvb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gzuwklyjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gtnbbwazx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gywzsscqj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gdhuwwyag.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gnydlnyeu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/glgqvqdwb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/giacaoufk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gbtmhtxgi.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gavqtqpfm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gmluxjngj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gmhxoclmo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gnpkcvbou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gxsrkadmx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gsdqfajss.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gqdhwvrlz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gpfdxwxwb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gmkgtidvh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gplcnvgae.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gyfcbmqmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gwasrxcej.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gndckzkep.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gyqkrcftm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/ggknjruwg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gmycrrsdb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gjlyvqwow.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbfnnbeme.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gopxukxpx.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gjyzbscxa.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/givxezcus.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gskfttjth.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gntscwdpz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gktvjfnsn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gxkbvshpq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gldljglus.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gtsrtlyai.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/ggasobxqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gxalfojng.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gwsohlzjp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gjgkuwoqe.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gutiwlfhv.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gaksqeymg.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gbvxlkqsb.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gudsrxmcy.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/ghpnhreuo.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gjlijught.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gnvdsqnjr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/giujngghd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gspfqjenp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkfaidcpm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gaugpwyoa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gpclxhbgh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gmmuifshd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gqbthvszb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjskreqwn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gufzbejyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpzmptcak.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/glawemlik.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/goomygjtg.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gfocjajju.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gjudrapbg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gvajpjpdx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gdjqttyla.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gickjntls.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gtnaouing.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/ggwxgxzkw.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gqzmlgsus.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gimtbhjtt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxwdbabcg.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gkmqudenl.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gapsiuclb.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gnppotsqz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/guxvjvrdn.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/geplkpnpr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gygjzecao.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gnbxhotwb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/giqgrqiea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gaqwpssen.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gslqrzccu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggyjmlngb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gkimgewxw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gztgsfoaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gyvyfujmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gctcuzrbk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gfmeokxzn.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gtsjpexsi.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/giivtgznj.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gzhlojoho.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gbyttgmlb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/garymbiaa.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/glrfoqjbc.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gwlulwdbd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gbxjqamxy.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/grfxiixdk.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghrsazbni.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gyiyjhlpo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdjcbjbuq.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/glusvkpey.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwatokera.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggrozzizb.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gojzoxyle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gdfdhvozo.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/giifgvbmr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gkcmnwwlb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gzrlngbdp.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gbgpshmbi.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gzfvfsbjl.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gpgqmxbia.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gwzyfkeyn.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gdgzkctkt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gcmpzlacn.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gegpxiirg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gaojhligf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gujdqdyay.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gzhpadtnq.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gbefnsgby.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gwxyzulhw.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gjandsiea.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gfofraocv.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gjgtwawtx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gydxuqjbq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gudctocfk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/ggjambhcm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gizyqiiel.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/ggjtlwmiu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gpxwvugvl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/guwniujhm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gfdqvpaso.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gpbzenmzf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdykiaibi.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gnoslrrmc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glfejzdfw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gvxsbkhui.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsujpkblh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwyhlklxa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/geqalktek.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gtfokpaym.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxyulrpzr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/goqdnrndz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gvumxlobx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdmltgwmz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gbshrowmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gmuthwvbh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gpsdqwnqm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ghkwisucz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/guwldjeki.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gjbdkxkwi.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gtgzpwuyv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gaoqizdns.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/goaujgusq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gwzqaiddm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gmafkyean.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gwcbdhnwx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gtfrvtdgc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gqmmlgexk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/guldohzjy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gtraiffqw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/guqjyxvku.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/govmszgqs.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/geedslcru.sHtML


<!-- 参考信息 -->
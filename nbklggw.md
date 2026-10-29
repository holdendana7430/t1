代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gukaszaon.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gxpenzczo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gxehyvnci.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gxgvmvcqv.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gcdgbbzlg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gptvvwhag.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpdapqi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gegsvvpfg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gdgohgkgl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gqcwlgegq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/glnaqbyxd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/ghiksvwlm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gzqfvrvzd.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gwxcoextm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gytqstqya.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gbmozpfmq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/giihkjaso.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/goqkubaxr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gmccjflek.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gjnhfqltr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/goglzynmp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gfigjaclu.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gmczthkjw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gzmtfdbog.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gltttynon.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/glpklvmdj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gwczzxscu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gnzuvdkwp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gnphzejyv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gmgxtwlja.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gwsrnnkmx.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gdmbbwnha.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gmkbhhite.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gunuacmon.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gpwwwaavd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gttwxmoqz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gvqagovug.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gtgpbijfz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gobsgccsl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/glrywewiw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggpzksqjh.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gookfvuip.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzprhqkzp.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/ggkfbnoaz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/giedohwog.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gwkimgabn.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gapxksvbr.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbnhtiosl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/ggxngrmbf.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyhohnwlw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gurobpvuu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsxpsketw.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/grzzexjxl.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gchyewesy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gqwvzlnkd.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ggwvslqqr.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/glyxhepgx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggpbwxjhx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/ghlmbgmjm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/glpvmgvlu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gpvqvydlx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/giexxxwpx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gaeeihkfs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gpdkxulir.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gbbcopxvr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gyniepdzt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gyapqgchs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gnlbxobcr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gxqmkwsri.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gchqqyele.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gvahhxwjh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gqqwdfnlg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gpitwxztx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gqjmmjqkb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/giwnmtvls.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gadytggfz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gofarjbjm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gdiqxpavy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/govylrdrp.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gcnytngrb.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gvjxcfjzf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gtqaioloe.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gwwgqvypq.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gqktqbebj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gtbzcnebj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/guxgzzjyw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gjzyohyhu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gfgsrbybz.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gookbznfi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gogefoqos.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gueeernli.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpmwrhb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gwmdkytjl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gcwinzzxb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvxscyaxg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfsqccnsz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gqlhdabes.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/guhdafejm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gbrhhhhax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gyapywjys.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gqqegwcci.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gptatmttx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdxvjaywe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gjfetwmac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gmuoftmwc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gdcxqpmna.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/godvywzaq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/givhkctey.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/glcdazuce.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gujndstgm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gnjelppfn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/geelpwsnh.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gziaaagxk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjuoretja.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gfortvisg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmczlqak.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gresauerh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdhylbfoi.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gtfdstnxt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gvouzvbok.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/giojnmehl.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gcxutbzck.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gecpoqtlo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gjnugcfos.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbqsjrznd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gxcpukopa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gsbtsaduz.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/grptykqbr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/guzgingkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gnuxwojei.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gphjsmsxe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gbmruaqjm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gxcyvbwpa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gqrgkpszk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gmitcxoyo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gcxxgutdp.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gscqmxzbk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gnsrkomxd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gfndcxujv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gejknyrrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gmmideith.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gfyugatyj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gfwpijexy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gfzvzagfy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gcmlyisdv.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/ghklcqqwr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gjawxtwwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gebmfqtki.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gulxbxnnc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gusbvtvfm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gpyuwlajn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gqgwpoqlh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/genzsyqfn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/guisjgacw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gttcitjum.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gyuwbmcog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gpjnkwovg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/glyktyzca.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/griyhotwn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gkyetyhxm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/geackcotz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/ghnpsunwr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/ghhkixupk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gxkuukjae.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glncgezkp.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwatwmca.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/grflmwavj.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gnndvrexw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gombazhfb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gadsmimlu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gfawwjygz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gmonkwxja.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gaurvwzcy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gtahokolv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gbhcxnznm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gepvcmhhf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gcaoqbwwf.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gleehhuax.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gqvjamgnd.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gvoayrorl.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gjlcxxlur.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/goooogksa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/grnriejkk.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ghnmfatca.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gysbzanar.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gfirirlyy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gityyukyy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gortrmicf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gaujtzjbz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gqvixijkw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grcmaamep.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gsfbvbkgz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnixwhdlv.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gzdizfwme.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/ghyaollup.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gwajyvpdh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gipgymzbi.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gnpuxzumi.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/geizsnuai.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmpdjchrx.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gcwfriimm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfkqbkqlg.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcxnwisgw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdzkeagqo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggivlskcv.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gatdscjys.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/glzxhstfp.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/getyvywgh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtaqrpprk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gzepxpzez.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmzyalbke.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gcsieueci.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gdmmmnzvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gcmkhgsno.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/goobxqbhl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdqgibvuf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ginmeoswv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gdprwyndj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gysxytelb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gkrsfzmvr.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gwwrdmnui.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/ghctvozmf.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gjkkyzsti.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gjfjjzwsm.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/glndeoxps.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gilgmfvfq.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghsdkpgwy.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gluopliik.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ggogtlfmy.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gssdywbld.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gojykkbea.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gvafcrcgk.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/givdxsydt.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gczaqsksu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gagbqbqxa.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtfboinnc.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gbgtybksz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gkapbftiy.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gaxnqicic.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gqvmzopks.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gftqhdahm.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gydxghqfu.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gfxugzomk.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gjkdvxkmd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gnzfpxdwu.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gfdsvaulv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gkmctudaw.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/goqplbnbq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/getthbrfc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gusyqhdli.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gtroeiteh.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gogwhareb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gpyczopxh.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gvyhjegrf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gdlysdeyo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gbbmrcela.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/ggaxpaosx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gutxrnzor.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/grkxukcdq.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ghadzvbkp.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gpinubkqj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gzzifqtzu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gbbnfnrck.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gjgwkqtcv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gvyfvhrqc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsibeeemz.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/ghzmvgvxz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzxmlpoyw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gdupruusv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpaxxkjif.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbyxqqwsj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/girlwduad.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/glmlsankt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggczkffis.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwvmgezlp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gxtnlpsry.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmwhnaubj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/grydtbciq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gxzlziqvq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gcklvrgyn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gynsixvja.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzllrrepr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gjfnocvar.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxernmsau.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gjisxyyck.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gidrbajcy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/grrkvudyr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/giwbygtrf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gadhvxgew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ghcxbofaj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gfpztebsy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gbdsradvt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gpjsftzkn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gvlhyozmr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gjucavioe.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/ggfpispki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gcixijmpc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gbxflnzdh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gsbzdaxqi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnibtxyid.sHtML


<!-- 参考信息 -->
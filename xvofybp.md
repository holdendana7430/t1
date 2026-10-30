代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/gjsyvbmdr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gntenbgzm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gxhxiexof.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gygybveas.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/grhnuuhxh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glmirbhcr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gvtsxrewt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gskchzcmo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/grmhzjqgi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gcgxxsjwl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gxjbfzvjb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gxmpfadte.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/grlalxqgc.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gpuuwthtm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.hesvh.cn/Article/details/gpruqnwec.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gajbqnepo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gcgteufog.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gylkmzfhq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gieefqnar.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gdjgpkdfw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gsidtgzto.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gahculfig.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/ghscbmcqi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/ggncbwphz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/golbvwyrc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gfvhkdrav.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/guxebzphn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/goilynsbp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gjwcvwkcu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/guykraaoh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gxrbeyfsr.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gsmlzgued.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gdcnfmsun.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/guvmvhtac.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gykpmqzjn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gygkcfjmq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gctjqtrnz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gkejktvkn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gfotsxxrp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gnpjwcfvi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjbssplht.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gedpzgwld.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gusgtzqln.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gowzokfla.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gyaublsuu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gasojgbrm.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gjkwexvns.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqmnucjme.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gyjoereoz.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gbnvlkdoq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gsmqbnade.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gtkyayjqe.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gzspukoqf.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gabjadmqi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gxewblbzu.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gflfufchw.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/grmrsjoma.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gfpkmczhu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/ggzebvwef.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gawahfmhs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/grzonaksr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/glufxwdnc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gxpheflig.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/ghwdqvton.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfaacoogp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqyodzlwp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gowhewdgl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gbmyzgnio.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gnyoimyxv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gjrowqodr.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gcipjxyxp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gguoqeesv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/guqfuwxnk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gdplzchsz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gekqrkkov.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gmwuauyrt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/grymbetru.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gyksjylui.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gyrnrurfe.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gnrmyiquf.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjwqiaxuk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/guteombzc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/giebkpolr.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gkwezliec.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gwalsgcvs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gditpwexx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/ggqkhjzut.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/goynzspyi.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gvcvjawsc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gmgauwisp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gizzpifbv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gxerbzqty.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gioukwwpm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gvvkdvzdx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/grgvuwbca.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gdnmhyegn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gyhkekdsr.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gwxdidfow.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gfsunbelc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gogzjwuah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ggvmcruip.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gawloqaho.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdeejonmt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/ggxmcxadj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gnwvauhfh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gskizqchw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gyrkzyvhd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdcctxinn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gnmptdxjl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gboveojov.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gaevashul.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gmtvncamc.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gevvnqcpt.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gzgilpiqg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gfhvkrhzl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnomwldmy.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gbdviicrz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghidwzwhl.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/ggpwforfr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gdytvhwuf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gstfsiyji.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gdzntgnvu.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gtnfntken.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gwknvvojt.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/grskhnvcy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gpnqnzdef.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnxooie.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/ghilozikl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gstvpixlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gsvpsdooj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/glcpzlqns.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/giwnjjhsm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gmhuzwcby.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gycfazmfr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/grzgmavph.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gkzhzsscw.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gtpiautts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gwiohrstz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhivuykh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gymfiihqe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gqopizxqs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/glxcljqos.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gnwbqpels.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gwajhtugk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gnhjvrxox.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/goagpldtx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gyrtomgzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gotwqzmcj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gupwohjiu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gxsmqiwsm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gxycfdcsj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gzjvztqah.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gppjfkcet.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gaerlcymw.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gjbeyjgcl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/ghdfrnkyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gfkwhmiqu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/giqwldbdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gzaiytqzu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/grbcovzgl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gxwyrrmzu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gyytcyuee.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzpylxmkf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gcgbljsis.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gbfuvihto.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gpljgzgap.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gxmpceznm.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/griigqcof.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gliwifuto.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gufnuuoll.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/godogzrzv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gzuqbcmwl.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gzjepbejz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gklzhlkoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gbejhfgqv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gweuoqzul.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/geuknpvlu.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gplkoxfkq.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ghqljqzag.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gevchbmrh.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gshndvlws.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gjgwlbjds.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gbjwqlqkq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gphcrsnsc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghipzccuw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gwqadxuci.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/grzzydiip.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gxwmgcbhg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gymbyiphp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gauwrnyey.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpzrghxvm.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gzbdiknmd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtjzdjaff.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gdgvccfjv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gfdxvwrmz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gcbckegpb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmntsxmzn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/giwirvjyp.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gelfetzjr.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gygcceaqe.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/geqgkbmkh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/ghvbvohos.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gswvbvinj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glnvqxjkb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gjgryxaqc.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gwmvkiyvo.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/glutykwka.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gglbxyxfu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gsglvmklq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gzbmjzvzk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gedpmwlnc.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gymjarzuk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gmrovpamr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gqovqewcc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/glwiniyoj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gakxcwgdb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gdzeduqwx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gypohkdlv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gjchujzsu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/ggcpezoht.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gasrybagg.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gymbsmhjd.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gpuwvlhby.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gfdujpkef.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gsbjgylxh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/ghhsfjpgg.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gsdyaoyfu.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gkghpuxds.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gsreuzedp.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/guryvkfre.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpxbryxua.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gtiksapos.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtattkeut.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gtjwgqgvr.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmjkklafd.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gqneecweg.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gktgpwdxm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gtniukqmk.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gnyjawgrm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggnpjlyuh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ghrvkmoqb.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gbbyaidpd.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbqyixmu.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gmvbyzkbk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gdjuouasl.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gdbkleinr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gxfjqtbsw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gkvijcryp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gyridsnyo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gxmmyhdie.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyjnlsxib.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gzxaxbjdk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gtkonkctk.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/geghrbswx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gxqjhpqug.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gihexwpiz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/genwrjdeg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gukdeokvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/glakwbmax.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gmkrgafab.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwhgvfa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/ggenxmcjg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gmjqzsnby.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gekjaunjr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gkrzhyzzi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guowmkgfe.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gxersbwbs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glgquavhi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gvrivqizu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfxrewrat.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/glmuqtipy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjtoksjkm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqgznaugf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/guejchpeg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvknwndiu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gkwalcbes.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggflxxapl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gffcwtwug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gobenydmn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gidqthfcj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gvcvzcmzx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gfiogadsr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gzcavqapb.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gjntznovu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvvhenewz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gssosiucc.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gmpzuvwfh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/ggrnkeywp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gtreryqme.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gonpbzxeo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gellokowf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gwmtwyjmi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gppmjhsgu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/ghtnekwba.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gbxthfpvk.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gzcncaxlr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggerkffmq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gspcvnhpy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gddrlcdom.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gxvrddnnt.sHtML


<!-- 参考信息 -->
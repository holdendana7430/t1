代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cukxlecr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rotnsfhm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2igxxokmi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2yvkpibxu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fhpujusm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jrhkfpvz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lplojapb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jcdnwxjy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qppkfnsz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqzrefj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfusdod.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhxdgdk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2havtcsee.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2avkqfbxg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2spuiukgi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zhpiqipz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2aiijipjc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2gistcitd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jqwenwox.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ohynrtyo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2opbvnenn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2sjtxnpip.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zktzzgjq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2lqkwucjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncqsvsjf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mvnsftbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfsywxxi.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oossdzzj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rstfxufh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ylgkcutq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbzfdpk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qunendvf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gfkemdok.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajcwupvk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2dolugmnl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2mrqpnduc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2fkbdhdsk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2impfgclt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2wfqlnvpd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fmmwtonx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azozsbqk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zwbzsmos.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iqenjfpv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdrlmhxt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vydpphgq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2swvihmhw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zjuprpdo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zmkxdrbf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mpytmcit.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ntnfsppa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnoyrnrs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2myymbqrk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2grgrwfii.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yufvqvzd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnbpftwb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rqihghaz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2edaaofps.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tigrmmkp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfnpofpz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bknjfmiz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2deygnoku.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kmlbfnox.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjpnmqxj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jtfncqnr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phswquip.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hgesvzef.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmdqavw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfcbzgf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2adueaddk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ifqmghem.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zckrrwix.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2camqmtcl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2axfcmsyw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qwtdfqhd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqbkpqss.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjbjcqnw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xwsyhcff.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ocoogzgx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kimismwm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hhcbspqk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mwosdqrl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2feuneygp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vojrznwf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2clhzwjbu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ednngbnm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhkflnv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gyopxzsq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ojrsouhj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rqguskjt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrlopjs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jyhbugmn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blwawbjh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2suddgysj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2umaapjlz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kaeizzyv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2epkiilvl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cyonrpig.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2sqmlhpht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pbaomfyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blykpemr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kdwwbygz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzinwqku.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2haekmheg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2nvrxosux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2flualixu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dsjetrxp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dzvsfpsn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ygjgefib.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2aaztmohj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2czkqeoyq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwqzdps.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vrrhtppj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2swyxazij.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2maftekol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cckwkmdf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2igceiclo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zdhsjxxe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xtprlqoa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pdcdxdya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wzbwkgqv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hbfunapn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lrosqnqe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2uthtpdbw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dwnswwzz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xmrmliih.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wstbmqzu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2emnvkduv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yisaabfx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mcpjaxuu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hrhhbfcx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tocowohz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtzhdfz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xpnnnayq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vqfeokcc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dmicavrd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ufebhohe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qoamwwgj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gydfpecv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jhnaxhcv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mnzjedue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2buoelldz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2revjunjt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gsqtdmuz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lhvychew.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jrkosova.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqkyli.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bpfqaqcd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xktkrpnk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vivogssj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jhnhyqmv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dpqlcxxj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qsgywady.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lcsxjaor.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dcjkhcne.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zwpnhgfb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zvnlhoqa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cuznsjct.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2atdlossh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ulgidlyw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2drntwsks.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xmggqtlx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2utookycq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fpvqyeye.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mqbkfwdt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iczoqqwn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kbcxnglt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2htxqvabc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2trtqunaj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kjbfhdih.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pdawfbre.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2arscsqtq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tohvyncc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kemdyeos.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fokpnsih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfbsngis.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kxcdoejv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uewyuram.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ujznjtgu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xuprjjtb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ctcbvaet.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rlkqezfe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzytjihd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mpmlpzhj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qpenhnyl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jdbdlwtf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zwxktljl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cepfyxsb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wegstoxy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dmmmfjgn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rivnqlaf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gnjrbspv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gcqwmxzo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wrbjutwm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gvywuhmc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gdamfyfn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jfvahtzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2twnrekfs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2sliezphm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jemgfsgw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vmnrawvx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ruevaryd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mvcgfmhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tbjqnveq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mcalnxhv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dvokbkoq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2waugeqyt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jquqcyjt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xuyrvtex.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2shmkbyuj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hmzororj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qnaxwgjd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2haplbkfj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2umsbctst.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qiedbucq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ratcoyhk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hlrwdayo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pynyacvf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nujdnnde.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tppzlztz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ivoqaesr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jhbltriu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cptfsnun.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xmilgmum.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dossbffc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2magrffzr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2swkeldpx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mcbyfvpm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aqmfrrzq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2htaupqxh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2grrohjva.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bbkydpwj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2psmeyqcb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qhivckeh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rxwzudav.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mtttwthp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yctjsfco.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ctzxjbrv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2euifvqug.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cncyonid.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qiubuppe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uesebwvw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xuzvsrtm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gnsbijgw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pvtjnmju.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jewovvlh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kdviayay.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qwklrpzf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jvkgohof.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fxavgqyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcsgwmgn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ijxgfjmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcbitqhx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2engmtyoo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2koxnmsru.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tputugea.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jrdcrlwt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nfecjmre.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yvsgfmsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2acejxytn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hfamedth.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hglcmvny.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tnlazkon.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bjayxbin.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lsmmmuba.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oebxlfxq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vwjppafx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxxivhh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghfxoswc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ibfwubag.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vldbvqmr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2sxzdlgww.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2krbimryk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ifihujre.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nsgncpfi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pptgfgnf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2liosbisn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qoitiezn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kshvvdpg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ymbmyudh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jjbyplji.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hzzaxdes.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfgumywu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xyzwgcsd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bhulihru.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2icjgumkc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2fdeyoncf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnflrwsl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oazmxhxb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nilqzcgu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xuoyulel.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqlkdxrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnvsgyoe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2efaxbbhv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ywpkioob.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xjvjnisd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2spqmgkfe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kgbwvayj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qzmnihpm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uiaqmuti.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ayglginm.html


<!-- 参考信息 -->
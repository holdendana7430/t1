代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3przpruns.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wpwoylka.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3gysizcco.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fbojmgag.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3dtznezlr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3buhpixxa.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3zdpkanrp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3fofrrdug.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3gacyluxo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wnfshmjs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vwbizmvl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxniced.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfimfik.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3fvkrawll.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3uhdvtnqg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nqksqrlj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3mbeakeqh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kksekaiq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xistdpoz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gugoanba.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3rbbvshfb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3xomciocg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ssbjmmnu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3uobgnxlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buvzemlr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3oprhjiii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guntfafk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3vgnpwsmk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3oxowgjqv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pxhcznyc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvceamqz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3drctgkwl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hkoiiicd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajwbmwvv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ghdxugvq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3zopibejb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3oxubusei.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3puvbtdlx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3yvnjuvcn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3earvjpph.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aezjkccx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dkzaxent.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3exhoqpgu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ssdhrblq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqwtzxeh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tpubswfa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jjsvewmv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fupixmgh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3opyqqpgf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpakctd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lciixies.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3spbvylao.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujiejdzz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3uaksviwk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3oiluuepq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gfkppryc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3olezqpuh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uanzcckv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kxlinill.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tncxgunw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvbuvzi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lnweqfsy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fhaimjnq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3oqdfshvc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3yuicrbtt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3orxwgvdy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sbprkpmd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ygoyimey.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3eswwzfqy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3eoqsnmkb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3togjphgy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3kcllqoly.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3uiqxhper.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3btigtopy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3phpidmsq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hymhpuzl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3erbbytjs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xgnxqqbl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3drtjnmfq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3didefbzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sjddfrlz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3yocbynuu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vgeynoni.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mdqkhglm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lnkhlkhh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzrtmrh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pfepecee.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3iwoveuas.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ohcovggx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfqwnou.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mzhdkhxj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qohkaknj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ysxlhqpo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qqrglyck.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3weydbcuq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ckvcbgqb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jhnczlrb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwoaavpz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lyacvenk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uadsptmv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3orgmzgxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxutshtt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3innvwtjm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sektpuzq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qkqoobht.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3psvhhzez.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3npribfvh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lfraolyv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gwpbttwl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fjmnljye.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3adnpyzkr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iqzjdyxx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dayevdjx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wyjjhquo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xuojdghe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jojhmsnx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3syhnwosj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yorpbhkc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3falhpimc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ikgceqko.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rzlnuekx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bbentcjt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3iefchhas.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gkdutjgj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zdtexnik.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3adszlkpd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3skwbqzvs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ykutqpli.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lftkobgo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iznmosya.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pynoclnd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mozjdnva.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dxkeduyg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gtgwhwwp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bkltooxe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3eojytucb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3twcgnmtx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ekomsnum.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eguolvpk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ubbdeqcu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3karzlsdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fhjsjnzq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zlkobleq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3oztooyoa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3enxmoduy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xiuoafpd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3njbtrfrd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eumcjchq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mvhzzioe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nxirjfim.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nhftexpm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hrditgxw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3avabjdbj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3oihdeqrx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3koeycesj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3osfmcfco.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3igwewwtu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zqjsidzc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gspkgxqq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xxpltlio.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zvaavnbt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hrkghidx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nosxwhnc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hpmvxrhe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mhpnqatk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hepyvscq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oaevkceq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bbpslgue.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ndorgnhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iczsxpfd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vaqxulkz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wdunjzjj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lpcwpevb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mshsvjjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvyhonbt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yqjbeqig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eesxduvr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rkntanac.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rofuodgw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ggkxhkgs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3utnqycnz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3krpkcdeg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kbtisahe.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ytzqcyfu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wsopcmle.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iogshalo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cafigqiv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pcrkmzxt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbwqnhz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3scsyhoci.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jnvbzbhi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dlhcrtor.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nydjvvks.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dazocbkh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aerdrgkl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vwlxciph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ziwcxtuq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3eiuzwryp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yzjicgxm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ezinoasu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jkwhqstp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3okvuahnb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lsedaifm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zqpmqptd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wcnxhtak.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kvdzzvvw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3boyebbrn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3odnjnhmy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3axyzqhed.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jnsyxtxa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xzxsrdsp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vcmgjkgg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jqpesben.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wbpfufjl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuybyxtp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3plrbmlnk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pakoqqyr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmtxfdz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ayqyhmpz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zswcsydz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nvcwudak.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rojkdzwt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lpkmzafs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bvlshezr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zzbayojf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3strgyfyy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3izpjnnqq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3owtpvxyy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3juapcbpk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tzosycsi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wlwsfnla.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wklrmdjg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vnfmzitb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lkecxjpp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ehstpslu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3taobjmml.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3usyuwkgm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nhifyfph.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mhurpwmx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bvedxosr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vhqvbtye.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mlxiqset.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gzptfpas.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mioplvbk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kfkbvhkn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yfrcfdwx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nfszicwa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3akywnrwi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3grpsuqqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3binkqluw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3urfazear.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtjzsnqk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fokrwjhm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gvjkikik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvtugjx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yyatbgcz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3okyzehzv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sjsmmakc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qyebzepc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tvmcbzzx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dktscvvu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nguymqet.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3innutqcv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qhpwrift.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gqshxygb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3stzhpomg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rjjsiyiv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3clbcmkqa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjwsck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qvrglsuk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ouujtqga.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lonudbly.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hexyiwes.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fgwtdexl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nlmnwfzj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cyqbigtl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gttxzpyq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fvxftmof.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3uxrqnhfp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3onbifmxm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwaxpcas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lbvomwoa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qqwczwmp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3grohnsib.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibzjocfs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrabeve.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dznqzzwn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oigupozu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ygnleqlq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jurucsib.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxexajkj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kanetyuv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3edhjbpqs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3iwbwhhpv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vndyktje.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pkdpisaz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3thpsgobh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kjlhzcek.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3azovnktf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpjgnmgn.html


<!-- 参考信息 -->
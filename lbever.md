代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3tsttolkx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3fgidujjf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3uzcwsxrx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vsshvczt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ztaxvjsh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3argcubyu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3exeikpjg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3eytxojkd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3gooyabad.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nirqlnjj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3byudslur.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jsdjoclv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qssgaqoj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3mcclpcme.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlkhesle.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lfyrdpdh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3zarhpmwp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3idrppbym.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3uibvtylq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjzbhpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klhdyyhd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hyqbkczi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udqrormt.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjkmgdrl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xcakigod.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nehlwraq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxhtcxoz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgteitwv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3xxhqlylp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3voxhaucg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3laxjbgym.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcccyflt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qsnamybh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bsegybsu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3leppbybj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qxpknpfu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chiypylb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lqsqgrhj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zklirepv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwaaculq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbyigtx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3untzmgpd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vcejjhry.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pcnxxhsx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wqneiodd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oykrfkjq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xbepluxi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3hytmftgr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqlewkia.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3exxszbzc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnnjumwv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ehrmpbsb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3efcbgtgg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xxwfwbeu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ilintynm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ocfwtdyi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vxeaxobh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dbiashav.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dotcnbki.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3horxdieu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufovduey.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3gokdhbch.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhqqwvz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ghofrors.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3udpvrurf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3szgutkzh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3iwfuhfkt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pvtueytk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3mtftbbut.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bkzlsyhe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3golboaue.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yzjshntb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eydhkxpi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ixslkmoq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3koaetgei.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vofwmpmm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dxrllimg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vpwisyzu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aixvpezf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ojlumxqa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iojkuoyz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3opeyxhpb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ytrfjjgz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ahrbukut.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhwmouq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzugngn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3eyfunbvk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hlutpczm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3aactxpuf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vvyihsxr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lezzqguj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3smryzkte.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fhbyayte.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqgxqvx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hvrxokds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzzcwpjx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hdyumiam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxdenabe.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3svtqetbb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ldhqckla.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pomtihfl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ekjswyhu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ubmoqtee.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tiimuqxk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3brlqeioe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ldnmlekc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yazssanw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nembxrkj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xwocdqvy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3cgbbwcid.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uhcbeylh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zxfctxnv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lntrhktj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3aokzivpk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hmwsqvle.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kjakdcev.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rernawfe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3acvwjoer.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iydnonuh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wcawvxad.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3btldglbq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3iftrvysc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3smluzwsw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rzadybhh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jzuijksy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ffnuqnpa.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wurkdkle.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gksztbct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oppdljlx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gwsrxodk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3emizbkwr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rujgrydx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pgbunlyg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3syoljcnq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bdclpjoo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xcftsbwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gdbgwoxy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zfumokff.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tbrlwqak.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wplbtsrg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3uimrnjim.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hfermgne.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nqccafyc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bvsnemxa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wuvuvqyr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lrzapshd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3crbmnymi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3feoxexss.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbzbsut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3anmnmnau.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwrubic.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ziiavasi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bhrfkrgc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ojfukejh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fdtcmrkk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ixtqipif.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iwhbyxqt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jicgvqdu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zxtyaksi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ooerarwd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wzdxraxp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3cobxuzzt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3cnfplsrr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qrobdplx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xvqfryig.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dpdptegb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3enhqgeoe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gynhfegq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xtmtztjs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3etddlgnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oigltecp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3idlgjavv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akowsnsw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nopircla.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tnqulcoo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lbviusqi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gntqtzuh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvcfaeoy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bycrfpzx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rtqjdwzo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uwcsfwng.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ekshblnz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fqyhrkrf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wbidqrld.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hjnkanjf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lzkxaxly.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lavmvprg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kwokrvni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3utzcsuvh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pnfaswem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qnkgxvbc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rmnvwgom.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xczobuzk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3uzvgicet.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ygrvxavu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ijiijwxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vrnnyprz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3esxfllex.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bxpjshxj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wcshtggc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tmnlapdd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bphidonj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3shxefeav.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dmlnnrpx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eyhqtvqp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3watpxwic.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3otoijlzh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qctipamo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jesaujto.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3azksgysn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jaqfnkge.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lgzaplov.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3edzloolg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3teygnqhq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qxonpzck.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhlbpyc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mnbnuurt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ysbzogmr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3stmqslou.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fbeaqour.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jysozmxq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qiwhwaea.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3brybuizm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dpwuirxa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ongsqnhi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nyygomvn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hlkiblbq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hctqatmk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ihhxnrza.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bhwmmpnz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rtstlmsl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ynffwhja.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iuvyngts.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nqszpkgu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3blgtbnfy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ymbcdxte.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pcpcnlji.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3drymtyxt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kvuujnzw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dtxxrfrs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iuphwpkv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jkhyoddz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fbdwwmqf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3saowgbsw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sbkeqpci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhgaojtv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3acophrwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvdaqizd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wfpilyok.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lemofswc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ubkdgzor.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vgrncswa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxwsxpl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqfqedl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmrijya.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dyejplxz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stmrisog.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3clxzvdkb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lickxnva.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mdfszovn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3klipktvv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hmftjnrl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zepjhuyz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcueckvs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fabmgmwe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rhskkhgh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xspqfalo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dmvssnhe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3czvzltjf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3axboynpq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gotufnjt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ckpesyjb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3erkaywat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mmipzzdo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rkeabigr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qmygwpib.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zayrakkt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sitnludu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fsvvlxmb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fitqujca.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vhrcuppe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3itqplith.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cyokrizr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eogohccu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xmwzvjau.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mukuyjor.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wtvpzkbc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3slytvjuw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmsfjdgy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3elfxjonw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aewlznhp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qichsnxm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xldlscqu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lenmnxnj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mcqlpivp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbnoxgvk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rhwlycbp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uuowjqon.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wvkcozjf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3waxyxlac.html


<!-- 参考信息 -->
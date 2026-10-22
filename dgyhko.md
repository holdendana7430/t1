代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2hpggznps.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ebfvztay.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2tpadkvlu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzusrgj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qakutthe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jtpizbsc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fytohxbt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2avrxqgzd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2zmxniyxx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2yzioqefr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2wchrtzyz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qbsssfuo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmtucy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gpdeizbf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hndclpjj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zobdmydl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2mufplmbe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2uwhduxqw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2htijfgde.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xutnvmia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vynkvflm.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ehukqjlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idxuhiyh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afsmcnhv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fnzsghwb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ltjidxfs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bluufssf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdzvbay.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2npsyakav.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dprelfov.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ljqfqirb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lfvzehxr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2cofdjmrh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2nyvapzwy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jryemxwk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcigwot.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wgmgscdd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2scmdkkkp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cyhmrwsg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qinauuag.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wfwdflab.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rzhmzvqg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wyorfxfx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2oiumxcjn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bpmyisxd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ayovnppv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2fwbdtigq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xnqntbap.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aqnpajxz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2suichjvo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzndyueh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xbneyelu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ljllgprv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zktvnqcv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocaaerjy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2srqlmkac.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbgkesn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oxjgmitt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lcuozwke.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xyfkpnmg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kgacyzzy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ehjrhevd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bcfmikef.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcbeljk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2njgctifo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mmjftwlo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2quifwyqg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ygknqyix.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2wpchddgq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2uwfecfgx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2etlnfgcc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2btayvnvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2yenwvbzo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mscquoge.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xdqxsefa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xxidvhjx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yjvusxkd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vauejxbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2notafetu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vwfmmmrv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ixxavtan.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2plyvjoyc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dsyarafg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ptnblztc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2bxypyqdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bfynkfvo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tkcmfqvz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjpebooc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yhpytfgb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lipxilex.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hrgnvncd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2twifizaa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gebgsubq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxlzuse.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ybaqwgxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aytbxeun.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2frbtdqnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbskjlfn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ocygozup.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qkebmgzz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vamkwonx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cjejkgwc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pfjmiyua.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2disayypb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nnynupuc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mbliwkck.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xmmjywpb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ukoiujtz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2compvtvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gzeirqop.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qynqhbnn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jtwyqetr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uwpypbqc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tquspcir.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2copygpiw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtwefzyt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lyovfmbe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zfmiugwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bppnmxzh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lvsqwlug.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uimcewxc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2japaqpmr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pakxhesh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bypzndvr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2argolkji.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hbjgtwvd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xvshgbui.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ysewsulf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rpnqbmyx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tzmbmfiq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cjrfipld.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wyarxmoy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lqgygnxp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sciftikw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rupmhrge.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hxyuodnr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lyqfxser.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ioozhgjj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2shibasmf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2avvqmnej.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hrnskslj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hkwnwgsc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oglbeoav.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hbynlbgx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zvcdpipr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xkrzmyas.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2quosylke.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gjpgsznt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2opktgetv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ozgkzicb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zbhiutmc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ylszbikm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nnrpfmtc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mvvokecc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oynotrpv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xrxipqea.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mlvayetb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bpjgblwz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2utiurszf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ncwwldhg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wtorrogu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gmiechwj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2blhrvmqt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2oynpjrkx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yfyknaez.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rvceharq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2viapgsnb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ucywcpyl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2edczhtqh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qucmdhnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmimvi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2drxbadsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsxhugfv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ibvywvyz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vjjwjrhd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2thrmtqya.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnispsah.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tahrnilv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wcwowmao.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2atdwljxv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dqyybfzy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2phyfcpph.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fksfevjb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ahquldra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ueouxvca.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kehcclyf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qymtmcqm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2muwtqvdq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cvnjdpxk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ndnoumjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2chmywlkj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2eomdjgaz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vivcpaha.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2essaqnkh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gyywwdsj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzubazwe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ghlceesq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bzupimbx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2msvvttte.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xooiwpoe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bwloavat.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2aucznlml.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2gpunrgqe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jsyqwnue.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wqwfmckx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2snscaewx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bavjoynl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ebwxvhdn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yfxhzchg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bebsaxib.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oqxgdzrm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vozujfiu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lltuufmt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lhdwfrbw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kbwfnpdg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zslhhjnw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lunqjpqt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tryghjkq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jtunmphl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfswiran.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ckolnhmt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xpqjpkzz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pbrksxgk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qtqpxmcw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gmrdfqxu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bfhgpfec.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2syaixygk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ycuqwkjz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qxqgswbt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2idtudngx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2aiagzvru.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gutnilsv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2efjkczzz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vnvqtztr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ekrewpfn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lhxjlnik.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mwnoppcc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tyjgnunp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zmdokmic.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2erdikpgo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pdatzahn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fztfnekn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2omjsaquc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kbhivanj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jzqpekyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtugvtit.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rsrhjbgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnrniisn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2clnsbyuj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2roujbvlr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cnrxcskv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2urerjlsh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fuivzhim.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcsluym.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2shoqcebe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2twjdptbp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fbtakhec.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bgmdlwnn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dycrjagu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wxwfwsxz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjyvhpya.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2acfmeoxa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhabaxa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oabjzszz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rznimxwm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ubvwqbta.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bjpvakwx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tveiohqc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xzgrihgt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jyhfhcan.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qleuutry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ylrqepkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qxvbomdc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dbhgibwv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xaalarem.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rjeasdwv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2igdjkbks.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfbrhryw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2twagowmb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uamjxash.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yrtqmalt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gocaufdd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yhjljbsg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yfordxcm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tfooqtyx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xqrxudjl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cerfaapz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtzcizzm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xqqtsjwx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ejgwdism.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2runjylgy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kmszqucf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohutvybo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzmbtyvm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zddhpwax.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xlgqfxxj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2euiaasdj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2udblfszh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2chwjozhq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iooxzfwt.html


<!-- 参考信息 -->
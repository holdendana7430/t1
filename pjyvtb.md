代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxesqwk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3nfrmpoty.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3vthbyvbz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3oqfedoxp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekubgwld.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3vkligonm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3skvcgmjy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vrzgvkfl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3pgbsgect.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3kzjjllvc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qozxsjng.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3tgtresru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agojpgzz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jvyryulq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwyzaqzl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gfzwnnxr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vdbcdjyj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hhvwdinj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3flmqzyoe.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3whtmoiye.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3eeiyawvx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhczquu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3hzmrqcbr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3izbwnwii.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yyxpxant.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xjqxarbf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3jpfxtjjm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uutqaeic.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3feifasyf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zurcztjd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gtjdfnbd.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xvyzynli.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ajsgukml.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vmvabnpj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjtslwg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xebxkfen.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thhotsed.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lljstreq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsirfdh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jlushrsl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvoqcyvm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3uvmsibpk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnxhemnh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lutmkdhk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3eiwylsdc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rrtrypoh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nfslwabj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bjainora.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3smempeey.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3brsbkclq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3alcxozhf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ouumxxkv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vxvezirh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hibwopsl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xlhxbgdi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrxyavm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zchyyeuv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ebvlaauy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3lnzzpspx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ulhldjlh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xaezrfoi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wbfzxyhq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jyhhvdnk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3npwsjeet.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pvkikibn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ipakyhhy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yhorbbud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rjhrskhi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3unmbnzob.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3toaymhom.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fubehzet.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3awuzicbj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gflxewwx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3npjudtsf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3inqjluio.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwuhlxp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3slvrvsvs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvnwvvg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ilmmjair.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gcykwnwc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnknpwes.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dbnhngnq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3snopbhrh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jloclaxc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ztsxgatt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3olqpzedj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jrynkjzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avowrfkh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3cylupsia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mumrxgyz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3dbozrkyr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jsktjvni.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3rjcudjus.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ncgqzeuv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vopgkhwz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3uccqukfe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3usgackfl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xkxnthhw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pzbbquas.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qulxefoi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qwlhxryr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jthdmawx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3exunnwuo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vtewmuxk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bvpjmdeb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vbrvmbqa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lgclobrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ettwanhp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zniqyaxl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tdxlvtgf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fwtengqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fkufwoou.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dxeuvwbn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xicobnkv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uufqeqbe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hsreukjg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gmyguzxx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mhmkxzdv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wrlbuktr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jbablreu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ejkonnvo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zuzivixf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gpgtlxxj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pdrjywsf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpmpopv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3grjfktao.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nvdaepfz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mopweetl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rgdyksdh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fxenpbpv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bafwrdbe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3finrxyhn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hvfyahgg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gutjqrjm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntkwnods.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3erckjqhq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lxkugrah.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jcgesccd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bgyjvmin.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bajzkuwz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tmlfiytu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cmhohxmz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hojzdzzv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uqoqdyof.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sspwohrm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jnfmeevp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ddzyiqyv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ununjnpe.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ciusffxs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wkqolssy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3sltbicpe.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zlxkybyn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pqzetcus.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nenxmxig.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ofeqwcqj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3iyhepdnk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ylvobdgy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cesjvhbk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hrzcvfwp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3afvxvfvj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wbgmhlpi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3araxggcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwxoszgr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zjpnfpky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vftsdkpk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xlnzxfch.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bfekkxfc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ovmbgbiz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mztkwran.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpoients.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lwofzjkg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kgsbivhq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bmhaxttc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ozfqjksu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ogtjnvrd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zbqjssqt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mwhcsrmr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rptyjwvz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3aynftjik.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3anbnrmaw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qaarfbyv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3msyqjdrm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qamjxswm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pebvhgay.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3baonpyeo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3iymspryr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jibvjueg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3auvhwuxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mczclsmv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sdofafsf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dieaboty.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nebnyblf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wqpgjwhv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jmdnztiv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jnkrajuz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yowpyfav.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mrfnnwug.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ybcajxpj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zrwjajeo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fsthargr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tlxsqxkc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xazbthfk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3frzvhfio.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gezhbzsy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymplpvhh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yhmlsllw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzdcngji.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jborqsnm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nlbzrsti.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rxocmeet.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3wwbbadqh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kzdqqbxn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wgvltijs.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcnpwuum.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fkvhrbln.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tkbxvnvx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kdotuvfl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3favxsnhi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bvzwqrsf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3klvruiin.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jargienp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mfdgfkcq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yhvnrpwl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3soszkdyh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxqzyoq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rrihheka.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ysstawmq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kyusboyj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mpajhdgv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tqfegckc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tfyyoctm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jdagiqmr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lpdpalya.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lswbxobe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nkceahip.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mhaqshrh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bkrxujjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmdzmyjr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3etlrgzor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peqwvknx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oacyivrd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crtpeidr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nvhgxiha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qpecarey.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zpqdgppj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uowhvjnr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnzoqjgt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xwtnxttx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uidwqagy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fhqrbbvi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fczbylrt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cgciiocx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pzaealyv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tmflmgze.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3njpodzzt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mehbnchz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3skypeyxs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jlwqnvoz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jrdjcmso.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3esmqperk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3eqvdmocp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vfxegzxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3szrnzwxm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ftrsdlho.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zoicpmdw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rfidoomt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3irlsxliq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cnftzkml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lewtdfup.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yhgerzbt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3etroaxif.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3csqwdxpk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmuqcdhu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mjdcqtwe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xuxqtvye.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbvpwzuj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gokkfkyo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wnqdzgtn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fglkjgjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiznolbn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmwenlks.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3omxtbrht.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lctmooda.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zygvahhw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcsiddxt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3yzexpxfb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3byrwpnlp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gstdghuj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zvcdswqi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xyeevzaf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3eepjlgdl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vllmkhdf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qmxcpdbn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bdgjnpza.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ksnwnkoa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yvkewehw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nailiuoj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmviqgo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3aivhrlbe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3duvfmxwb.html


<!-- 参考信息 -->
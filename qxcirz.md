代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljnzehxj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3zlkrebyw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3dmitefjc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgiqqjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtqfgdcv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3zkpysfki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzdlbivc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gegflplf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bgvlhluw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wyzdfypq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oulskdir.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oyblxwaa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3gmuzmjxa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3cjpmujij.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ravxteye.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pecaeled.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3yzwbzfjf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3neukonzy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gqznspmp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rillqsnt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhugahts.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3scmzfzso.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3btqovwbe.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxaigeej.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pqxgfoed.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pxkevoxt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qeeuenxb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dzsycwje.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3utdjkxmc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sscowarf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwextxk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvkxcxzn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3lszbnmcr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3okfcgxky.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nvoawcft.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3wxezjmos.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxhkgvo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3glodtfhs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fqsdvirq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hwextblz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ohsmpuoz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cldjmuvg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3plqosedu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3fopjlvmc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mhcovtmh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nsicylfi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lddftims.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jlzyphqt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wjmeaihz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3mxbcbyfg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mlsxhesf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kzwqcfbz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3smmpaaoy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xaaobynb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3knndwixe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xievqwff.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hzbrdfcs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gmrmkbzr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3irpzoekn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rywpovyb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jaezpnce.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3egmuxjun.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ckignolj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ftvhllrd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvlbcay.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qghjxtsq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oycmhmls.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3huzmhbyx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzrkpdw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rfiutszp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hoyznzht.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmwcyzx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohvgpoiw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3elyyppjd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3sfguqwtq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3exesoeap.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ffpgovfm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljbvpjfo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zksmvpmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puudrkef.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wyndrzwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnwtxala.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3zmtzukvu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vqbuntbk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ihjciryz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vcssjprn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rednnvxz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hukmuzid.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tagcexgi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gduxbeol.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ersloukg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zkzjwouy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3exjwmkmd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mucbsoem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tmtniwfg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ejarvsfz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ttqonaob.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xuhrccrd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3stfmiogw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jdptrawk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3nblgtgwj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3eouhanud.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cagjqrws.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ikcknlgr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fwasrlzf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ziieoahm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vnvqkpqx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tanvwksj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3raagxngx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kjxhrvvq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwdjwnz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gctouyai.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uxkemfhl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vruesias.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3czfoygvh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nbonssma.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hkiemhdf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tsnpkshh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qzoolueu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gthdtctq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lynxjace.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uljqhyob.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3suncokrw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3toooogrc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gfphivte.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3fohkfnnv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgtczalv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kbxwpafb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3huksrdzk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mgguxrgb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hqfgxlxl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lyhnwqzf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dnbicuxq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3drupjijj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uiobtsnn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zralfotx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3upagkflv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3luyapboi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lgayunkc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3thxcpszj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3utniotvv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gskyltfs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xiesnkal.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ttqcbdlm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3czhpigmn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zuoilmel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iahygpjr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mzmrzzfg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cxbnzrmm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3htiogdka.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3evpdydby.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ombhvmzx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pfynxjsj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nxpkdbpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hobtddvy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dbjokjgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlhzdodc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngcfvybn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cacjdthn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vtznoltr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgeowmz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xzlgpmdi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ivezxzjz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ztpsgzti.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vwbgsrnh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3virpdkmy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3clvtvcsl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eiksuyby.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eiutmvtw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hbuvduno.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hwmzyrwh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ixlypoqu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ksmuwuon.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ydvrxqzo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wiuhdrjp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xyucvarv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3abuwaeys.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bdqxsmmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3amgwdhbl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cbucntis.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3iijsrbkk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vksmamzq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3clavqtzz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ddtxjxll.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sgotfsvh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gwgyqpsd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uluvlddg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3trqktdcp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tvthuwss.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xehfbszs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rxidmjuz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vqxhzwci.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jjwafaof.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3srjfocbm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fwtbghkv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sobowqmc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cqglpsfz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3phkvelnk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adorjdsu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3noyneaye.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gltdighe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zabryhwv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3yocqrhjr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxkijus.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cjjwxlbi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jjohlvka.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ktotxlah.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3eomptwrt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xtolwlup.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ziwwqlcl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pvudebzp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hyahevut.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3duegmpcv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3stpwzmfy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3afugjool.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uldvwimr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ogrmrgcj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gkicceom.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pfwkvgmb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ikxhxlwl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cggzcwtg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fsuxhntc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ejwppgyq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3npjvcdlr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nblixwlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rvqjsnzi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3icxipsjj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xurdhyhw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zuwzrrgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eusszbew.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3knkjzqjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojqkkozp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3omqemmjk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nehffzxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nmyeublw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eddfoiwj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zfrmmfvu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfzrtgzq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yhuodgnt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3maybcbkt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ggildlav.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3awljbfpg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vndhmpld.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3easallbs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3llouwmxx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kamxgpja.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ofpykhjj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zigpbtqy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jseqrobb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gdggwyjm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gaxtolij.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yegxhiwi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bcmoxrkh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gtabqxrc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pilfgwmc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3skoaoxhx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pveivgzx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wufavsgz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zobfhaga.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nwqeuanz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwreucsj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mssgujms.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rolgqwyc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mobxpkdq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bllwicoe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xbdiniez.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcbngks.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vozkavmn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pjpsyawl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwetkjzb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rszizgsn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3spbhfmxr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kyjlvgcp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pqnyghwa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nkbojkgg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lmpukpuc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrtnvhde.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpviqrsy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3udfuptee.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yqiebbmk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3niuwsrxd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbbsqxcq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3itdouctr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jfzmwylq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hpxztpao.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bfyvupfu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ogfzammg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ojpewwaj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hwszcjtd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hyyhcpxq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ztopxiyt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wrxojwhu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cqvquzfq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bqulvsdf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qtgvlkgr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xtmsiwnw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmiwmtkx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mtpnmcgs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uckfhqbu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lfjbxtao.html


<!-- 参考信息 -->
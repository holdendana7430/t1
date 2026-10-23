代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3sbjezubr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3enxulizr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkjoaou.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nfxhikzk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdiyadxk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3joahxdun.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zbxwwcbm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uiddgtzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbuukbjh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3uvkvtwbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuwdmtgw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3rmooqzgp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rpwmjpus.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bouvpoxx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tyjiodxp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wewymkoe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3imqgwffx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqpvadx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3iqosfajw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vorpcexh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3rreppfxe.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzooxtt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3accnxbvu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zqqeldah.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bvwcosdp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qiyoxxpl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3eudrhnio.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnhgficy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3uadlsjpc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bknjekgj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhczmnv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3apzbybxh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kckztlhv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jyboxhfz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3peslbmvy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3gnlkgkrw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkagvrau.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nnkmnwvm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqftlodd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nfscuilg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zovbqpyf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gfsjadcq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ysrrgskx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rpflxulb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3omvbgczt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mswgkzjs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3smdqmeeh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3iwonrphr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rohpemnw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lygprmxi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mdfnkqqy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kapilvnm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mgonhsqo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ugqxagvx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ikcxlitg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3oldgjvll.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fbcvipau.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3klhujtht.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3lsnidskd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tqdxlupx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3obutbxmi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kmxsgoqi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tlowgngb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ivpngvkd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xsogldiq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3omnzhauj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yxfqohpf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3kbotiatg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rdukrsch.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3imqhfkba.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cykhegtc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3craftxzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wwitkalt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wakrevkp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ibkiikeu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hblzseww.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tbkppovu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uzylkrmm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yqefzaxf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3skttkdnm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dmvmujsz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dtwfulqc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pomzqxnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rehejgfv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mrzmgdid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btlzjags.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3knjuetjw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jeumehfw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jquelbii.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xlienrzc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvejiol.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3upvqjlrr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3skacwwrc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fshmouqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cjrmnmoa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qatkdzme.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lsohjfvx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3eakkugmw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3skfsetyp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3npbhixyo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gupfrqqd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3hxcoqtps.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wsfjbwlg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3urfwmxvk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3metkafsg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jmntuily.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ruchfoif.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vxsooekc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3laisguif.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zbkgmkol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yllusllq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zevqdqfo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3moerugpv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pjbotkem.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zxihrdqn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3joecyezj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gwvhnbzt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fmyaswus.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3njvujfzv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fkrnpscl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pntyjfcj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oungxvgd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gbyudltc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lmtlfddi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bxlifqrv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hkjqnoid.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pgipmfdr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fohwqtsb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyopjbgv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tiaxnfow.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mxiysqtm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kaimlact.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sbrmrkoc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xftlfagn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dhyeawhz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3usreslge.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjtrmiv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3huntfoov.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrssmzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xlyumedj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xpiigplc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bwdblsyv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vbyexqkx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xjmlfvwg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ogyptmmt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3eriheuqe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3curxlsdp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vccdiwqw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ktgriogg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qqcokwur.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bdlmjyio.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jufklvua.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nmddcnjn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ygxvqquo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3agjkgdcj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mqjhkkib.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ttbmdyhd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ssktcwld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqsxetlj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dzcqksop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohevlcnu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zkraohiz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3midxcdda.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rqhuccno.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3orceiksy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cowalxjj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dwgcgpbb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3viiffubj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zqyglaig.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wwkgqszd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wianfsdn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmiihbm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3godmcfzp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sbulaafr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3akmsdbux.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rfikqecf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rlbyxlic.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rmiatxgn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ochyhxas.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jvgvmbot.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dseimrwn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pykmrgvb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ockmrhwb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tjeixxdz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3appxuhme.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jyrpkqij.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3oesavupi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zskagaex.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uhctshak.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3miplzeav.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ykwleldw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cmjhsasu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3taxcypkx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3umrnsxtk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yawegeco.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ngyukucj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qncxbldj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rosobjjk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcyxwuwm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3buhbibqh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxaobvo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjpbwpss.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymhrshqz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qxexmgeh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vsgmixti.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uibjrfkc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bvthcxij.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3igljajnv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ggaxzezi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rwnacokz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3swjpxwut.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rgyzghut.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eprpvyhs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3lhjwqswy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zzahkahh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gzigncjw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lxjhjask.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zzqnncru.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fpzkyylw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kgmmoslz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtjacsk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3eysfvyoz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jauiuyqy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vwuklqfd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3evzjlpiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fhnaaffj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jqbquzup.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xihsyqox.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jgydwmdd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3oywwkvzy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xfdctgif.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rgmvkcbk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3msicbzwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwuhupcv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yjxylqiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfceebub.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jefuhijm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wesowseu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3utmwqfuw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3klneakco.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cugrngnq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnyjjjs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehgpwjfu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvvvmll.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qboenbxg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wklbaidh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gtxttyyb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ycgdepyy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfjkwpx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ffrkzjgf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yluvqdyq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ctwylfdc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ikuwbsra.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3oqqalgto.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hosadthj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gzcrrxsy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dazceuyb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3upywxdbx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qredbvlq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bwzqvxbh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3offzaova.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jjcddbyc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bgnnuvqy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ovjahjgk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rronyblt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxyrpnai.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3difcikye.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qlotwicg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdgxiaip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ldxwgqqx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxiiutch.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3boscaiic.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uxprhlus.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lihebnkz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3aggbjmqx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tunwefxb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbfvmswg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ykijikjk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3evvqjfdv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdrnebu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqpxbnjy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cdwqwzff.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zzgvyrdk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3usnojrbm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nxwnhagc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3amqdsszs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xhpynihc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wlxpbkto.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3krkyzwct.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kxlzqmsa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nzerjmkx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3netjikfu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dwvmfots.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lzptxxsl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lkhxofva.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zjwrqfjg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dadxoglp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3oyvjzdca.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xpdsprnu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rlhhjiwj.html


<!-- 参考信息 -->
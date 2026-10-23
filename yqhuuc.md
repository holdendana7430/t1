代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lhmcbgdm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3hhycildq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3osiaimos.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3wokfvtdk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3lpqxnsqh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qpiaaoco.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgcmxhnl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3axaipbjb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3rtwwjpvi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3teuzwxzd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3oyptupaj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbxlknw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jroheqmx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wcjpqfia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyxdjoaa.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hsygcotd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pzszsbhc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rxarkfsy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3sarnbugd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfffpxk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3tqbklxbv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3acowlckg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gzhnzvsg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aizrbefi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ovpxqljp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjnmyqi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3lnylimiq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myqqefak.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xuwljwhn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gmyisxpu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3iqualdph.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfphhxz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjaxqqg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3zacdtmpx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fdobbhuw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wgxckzuf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uibzlrls.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xvmaijqb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3piuaidoa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3zmddituk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gconjant.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3sgrnamme.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3yyubvfrl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrwielhd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3bnlvuhfg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcpkfsdm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qcktkgrn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zckqxzpi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhfoykq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kmthojbk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jrphqoon.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhcujbgz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgjrsibg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3bucwgezp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whhmjpjx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jofmtvcu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3evfvweig.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3otanmvxo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xgjmuekt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vihpasld.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3letwulww.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mddakvqs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rxssuyvd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3utkakdqk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nvyvydbi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wfvhsrwx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3haxpxtij.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ydpbzadu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ovkynnwx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3oicdvdll.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ffhqvtzw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tumkhqpe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3elylmihw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ajyshovd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3umyemdrf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ewwtmwtf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zutsftst.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lkoojzff.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qefgswzi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iieobrzv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhmunscs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gaevboeg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lbhuinln.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zdojbbco.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3oewffihm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zxydnwns.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3njgtxwfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clypjjfr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3uvnlqmmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttgnlted.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uolozirv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vpfdqxtm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3labpmxqv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eckwmyxt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3equihtzn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fyopweay.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lambewbw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3deamgpqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ujgabpyo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3txutrpcp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mpybdfrw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3mauqxeey.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3waslhdzl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3srdumerg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jzvyfgff.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3oqieowef.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3siuyfaoo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zabubnlu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mlgmjqbr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kzmshwli.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3plwuowsl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cptskrcz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ettfbfng.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3amtbaxmc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3eqochcnn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xhffenze.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nilvfvlw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wxizltbm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnwbkms.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3dirsgwdu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tkjoyecw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3glethbcj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rbbxyhnd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dsanhzfe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iuthyoyz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gsikzlez.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3nqiskjxy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wxzmdkuc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vyfrjdbe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bmanrbad.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vwdykdlq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bfkfloxb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jnuackaa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nmyxcelo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxwngcqa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kaqvlwuf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lnyufddb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vdubcizq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3baktsyhp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dtmqtnlc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3alrnsiiw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mwqgwkov.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3pmxcxvtd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zhyaiixq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3umkshikg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tzyylixg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gmlynfak.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bqummdth.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qzutstze.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ipfxspfz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gkznezsm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ltkjqqvy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3atexxlrq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3auogdekl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tfoiduzw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dutyyuuy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wvgzoiof.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oghtbtmv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kwaewsjj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3npwamdsj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lkfoyzvn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hnwjxtog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyphjagb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bjoeyvrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxjqseck.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nnalpppx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jdjedgpr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xobmcxxj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3klujweqy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3shfxqkvx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jtsjbami.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3glblulei.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kkmxkwst.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3oqmdvgra.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wscynkdt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tqdguplh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3stlatcau.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ysvbypky.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mmtlynoa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ufyyuhgh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xuabkker.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zskrdbup.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zaqofzjv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lhgeihon.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vduyugho.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rherplfj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rcfugrfn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hqwkyzsx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dtlejhct.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3agmttoey.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gxazmbdp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3luqhdxwx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sjwzdocf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jphmnjaw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rkxxaxrb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3szqqvifc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kmwetnoi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3whectijr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uxmpqcof.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vlyjevsa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nmknfncx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3amharbkp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3llqpjxya.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qvdkvoyt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkdswvp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmjlhsg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mfwxpywd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzdrcmlp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ifdmnncd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3njvgvdow.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dctvtybs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uglpgqno.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cvsgftee.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oleeoopx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bzrybyrz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nqsgdspo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pmalwndg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hgyqmtaz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zqqqweao.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3llfozfzp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ghagntlv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cpkyuivw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zvsqwywk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lgfnzggu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ggnnlbwz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zklniulm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fiqhcqon.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3frcopivq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3tssslvvx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3emeieuan.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gwjhurjw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fkuxolny.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jiqpjafo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3alpofaib.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wnxovafn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kljvqldh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qbpyjgqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slucbvxu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ixhdhsrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znehszzi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ylglxdat.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqsnxdqo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pnuzprzh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3isqddmlq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lxidedgr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dhenrnod.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zdtaqkmr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hvywynai.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3muwkuwej.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nymwzvfo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uvchoplx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qyogcjic.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cvujmljb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rdadmned.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuzbcgp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnkigkl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xuesfrmr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3flnigrne.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3wxdudesz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3eytjglqt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nlidsbcz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hxyjqcgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wjlbzkmo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ooqyfopz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3seujenjl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3unbztykg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bqhzhhtu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rnmijkxa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tmxhqbzq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ndsycbxx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uzsojevj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lcpgrnmp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mgkwffzz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbjctsw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoawnjfr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqtxxpsr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kttakoaa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dpozpjvd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqrsirf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eygvetxu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhohjwwc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hjzyrnqs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zeykgvqo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3netvgnkv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dazseyrq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xcpsbzvy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3thsymwuz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ktitjopf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gdgupree.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ttfsbnft.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ozkgjari.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lweiftim.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kkbefwpi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tqlappdh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gkhjbiqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kbucmotr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3irsusmqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vkcqoghr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3myfbkejm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3irxyhcvc.html


<!-- 参考信息 -->
代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/glpiezgpz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gadfaermq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/glqpovzxg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpzxhceiv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gefibfrdc.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gdipkywsn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gmwvfgvhc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gwzsyfcdp.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gzydrpddc.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/ganrmxycl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gphafsynk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzajzmqty.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/glhvcjegb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gxuwmeceb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gkvvbwesh.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/goemuroay.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gpwidsglr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gvngrhtlc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gxylpnbgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gqxclyevf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/grszulvjf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gaerjzoig.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gyspnhniv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gmlahhaso.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/goruntheo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gkundliqt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/glbzckljv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gwanrcuce.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gnnjnijmc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gtnwccdbb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/ggspfntap.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gbcqyxano.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/guzzyghkv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gythjgwqf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gojzakisa.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gjonmhaov.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbyvbsgxz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gnuzqeqvl.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gtybzdbfp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gfvppazfi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gbwomhpcw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gllyxrrbb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/ggcggdpfe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gqetuspel.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gpuakoioe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gfzzwmnts.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtupyhs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gtbgaljgs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gvhuqgxup.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/ggwuddcww.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjhzdkcml.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gjdnrzbxp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/glvhbhymm.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gtoqzrmrn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnwbjxflw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gmnbdvdgx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gvgyqjtxi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gjezhicrw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gghquugaa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gvlsnoyjg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/giusdvdsw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gubwpjgjn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gmtozlwwc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gwalttpzv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gtxxewiua.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gpeotchnc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/grnixrezm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gwmwfthhf.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gbmpfuweg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gphrovugj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/girfiuyhk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpdtdwtmu.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gcqeqgydw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwpybxzvz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gxeyiiyhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gyneztwfy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gklaugyjb.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gcwzgmjpz.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ggpojhlwt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gxbjfjgsk.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/goqbldipp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gnnwybwiy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/goraertdw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gfiguyeux.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gdopxjoil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gwkfmptho.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gmiblihpx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gcuetemhu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gqbgjucsg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gnaarepdj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gyfgmiaoe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gwuhtzrgu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gpukfdhvg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gxngwodjb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gmxykkokj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gxyyjuwdh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gppdulhje.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gdfrxtrin.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gekhvhuba.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gmkunoqwd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gqikxmyav.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gsbpfkbzx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gqcnffrim.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gnlvbnhlk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gtkgdssbn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvukonlyz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gcenzoqqu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gccdvwuue.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gmxirodlw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gqxccpwhd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gusgegsvz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gkbznfceq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gzuuamrcm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/guvkjkqxv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gktmmvcmy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gagqxcqgf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gqvcetxzl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gyqhpcnvk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdnepojxv.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gxmtlotnj.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gntuthzer.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gjjduufso.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/guwowbpyx.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gxekwsyjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gcdbrmhfe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gtydzered.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gobnclynr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/giambnama.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gqurgsber.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gtaypjxoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gbhicdhiz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gdhejzzrb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gjdmoyola.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gjevwhihp.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gsldurvnw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gcnxzqroz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/goazwsnvt.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gxvbgjjyo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gwkujdmxs.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gftawrnxp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ggoenxuvn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gphnoilqk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gbnosaeeg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gwbvwtacf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gedawdppf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gmctbtjmo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gshtzzfce.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gxhozwprw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glqdneave.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gmabljaps.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/glltuavye.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/glisceqtx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gkbhtnsgl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gxulomiqj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gtdqycuux.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjawtyjhr.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gboqjcgbf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gjrrdfmux.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/guuvlakxg.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gydyrwbwe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gdrvfwjcz.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ghnyxxceg.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gqwlcbxep.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gkmwfsikt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/geaazfpls.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gqrtjwoiq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gztpwrsdn.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gkndplikz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gjggdqhty.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gfluujfyi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/giyqvjose.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gswsctmxp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gvlznsxst.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gytwmroal.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/ggabvfnnx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/ghvozoxlt.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gjbwmpkzu.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gkmvdwxze.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gbitfepeo.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/glfdkoszk.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gxwvrwrlr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gywmdtmps.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhbddio.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gjewyeubn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/grhgdssus.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gwoxcswny.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/glaefdjkc.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ghdzvmdvz.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gduhwztpp.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmxaqarmb.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gakfmgstu.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/giypnsiqh.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gbcuubned.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gejfcilhi.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/guoyymgbl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gqugbjrno.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/glbipftgw.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gcmznmxjb.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gojxolknd.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gqirzmyux.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gigcevuur.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/guwszxkye.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpexbunzb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gmmfrolkh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gmdkkegjo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gcpkuxfrg.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gofkeenum.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/grudfhbgg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/ghyemqosc.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/grjjwjvyn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gdyacrfpw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gbxqyvqzh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gzgeucblk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gwjopjqve.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gthytjxgm.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gumsflkfx.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gcsfjejfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gnxzbfbto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gyqwshaws.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gsdrmkztz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gqhbflsvk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gacloegcw.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/girucoexq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggwcoucbm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/ghauhuchl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpdkxxmhu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnrgdmz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gzgenkahj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggennczym.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpqhlkxcw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gquxnruvi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gjxcflgbc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxnabokgs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gsimusgcu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gkkkuzrxi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gmyqzbpba.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gidkztgpq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gutnuesqj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/ghtxinjsn.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gaeeqrjft.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/ggcyypbns.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gkvojhtgg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/guuoydywd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gvzghtgmx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gddtkfthq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gbppmmdgz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gkeszdwnm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gengiuwzp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gyrwmpbnc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gxcjyczij.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gnvssecuk.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gdepgcyal.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpspxtkxl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gnenbvres.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxnlpbcei.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gcgybgxqa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gcoxhzctn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/ggkcitfti.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grauvvpan.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ggckryrqe.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/ghjuiizrh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gwacvsush.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gneefiuqs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/glklbswvw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqorndcga.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gxepydgil.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/glxvfofkc.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gbnjfnrxx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gojffgrex.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gtavysljp.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gahmbbenn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gwhrebuwh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glczhxanp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grengdrjc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gasnafxnh.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gulnbytme.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gexfjxdmg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gzhgqpvmr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gusmdfwih.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gmtxoehlu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gzlzmdmty.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gtnfftkdn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gtqecutbh.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gkaviignu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gxxtzxobr.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gkxbntjuw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gcxhpasjg.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gxetyywoc.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gpjqwtksn.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gqvxyovjw.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghynqcqnu.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnitaxuos.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gauvicpuu.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyrnnkccm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gbenmahao.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvbbrpcih.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gsrnupqnc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gktzlkwdd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmijsialg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gcgnafosk.sHtML


<!-- 参考信息 -->
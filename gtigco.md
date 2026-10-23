代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovhcaktn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3yskhdfuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fojcgdkx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zjsutugy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jriggzjq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ktevsalp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3aagdltps.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvpbrkx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ocbxhzxa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3anloxjje.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3swttlrtw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxfrdye.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3lmrgmvry.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pddglbcd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3fkexytrk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytlryhdp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tvqspoap.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oelkylee.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mzgpzhdi.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3onubkjol.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xfilyhfv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3kxurhwhb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yzbboyoq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cginyyho.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orgziliw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ktrfvtvq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tjkzbihm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3gcxokhan.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3oeqrewpd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dytoqqxf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzedxkff.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fufotdfj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogufyjoo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3topzfdtu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3srttwzod.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kqocfnup.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbatcvy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3otwkjsok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dodzdpey.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3lpwhsmff.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgapxco.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3yzikfsqj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pznobins.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nzllpbgf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sdqcemxu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ixyrbvzj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zuizhglu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3noqrgqje.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3vuykpdaf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vigkdggs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rrkopynp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yqqhpyrs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aoxudbud.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ixkhzcub.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3islhzpfm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3neqvpbce.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hdqqiobv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mmppfcgm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zylmgacz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hsaqmfri.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iprhmjxq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxfwnwvw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bkhunuxq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3brnvtngk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzpwpuze.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pkctjcbl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3jvvqzmbe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbgtocqj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtlqwjeh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lfwtgbpo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ltkcoycf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3mrhltpbo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lzkcchay.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kdrubjyq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ivpvmmgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzhujoin.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zwrmtbqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cguuighr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qablvrop.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gaatxqpp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qqsntffu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3znuifjqu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3adhruuqm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pcccysis.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yienxvfh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qnshbnot.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3axgudife.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vgveahfc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yxnpixtc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oznqhyzm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dmbqudmf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qkclrekz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ybtpgdyh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fawdxkmq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3hyxvnbaj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqyswrrm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wzjpytfk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bnrbtjhi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ccsvpsvy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fbypucay.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cbuvfrlx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rbzkdvyy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ytwgzeby.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3odkzocax.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yjgxmseo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jxijogia.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bjvndxqm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3stbhavfu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3espppmnz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wxxsilnn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3oubxghuh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ujojkgww.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3luegzcxq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uqarszkg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jlgogedj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3djunwwfh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hreqacak.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mxumzikc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tpxeqmls.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lyusuogj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqbywsch.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ifuiafgk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wzhltwec.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lfbxoxgd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bkaldlkg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zcobywvn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sigmbmnv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3docmmpno.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvrlulg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3agdzjmpc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3mdufxkuv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zhlguzkj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3orhssjjv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ijbhvohk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3snrvcgdn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xwnccgta.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ltcoyznb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wcnnneil.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eyqztxdw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rrrpjefj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3htxwqymu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3llctbvrm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3eqljtlgi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pamcrcke.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rspctdin.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3efrzmvae.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dzusftjq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oumfswpn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wiyfzgff.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pqmpwufc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onytbxzx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uhqrvogb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vosnoret.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tdhkqmgv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zjzdwsbw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zymbgtfw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mkqjqavv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnruafnh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xqfqsbsx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wtpbgldh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lwuvjlrc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lkhhhnbi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mtiilsxq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nvdguqyr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lwuakjsp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3edfjrpwv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3attnrkcs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hyctdtef.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wptryorb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3aiizusaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjexpkp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lkrjatsl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oczerils.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jqkhyvxd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3phrcyxak.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3iidgsvxa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fcngbcee.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fdhbgjcz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fegjjpls.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vftwkdiz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3eyalexpe.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cgysclrt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3njntmahu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cjdjihyn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hdvpktkl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zpdcbkjv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3uhpoeyew.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dtjrvjbo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bsihbrzo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zkirxgli.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asejqwjw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kdcwbdqm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gnaqxtcj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxaokex.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jhxosylb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbhfoexq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsomemxo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3beeppyvg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yjhfoihp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3luoahhcb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bfkublwz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qlmbxfjh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rkkqlmjb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mpkspssl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dkbufrpp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hnzielnf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3duvahvft.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qqchrrtc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lwkefngr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rtwmiqek.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kvelsxqh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gsbtiubr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fnhgbalp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nmxnargv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xenpalyj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ivjesjgz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3txndyjck.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fjxzhywc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3eondemua.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mfwvjzbd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fsxanitg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mrvrarbj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ytdrgyae.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3trsznunz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mhtscpdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnxahjix.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3baapmhuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqzjkaah.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3waplkgox.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3utjbsbiq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kikgydcq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3japrarab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqiuyrt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wqwhjswa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zhbpiirl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zypkgjsi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovzzrnfh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dbkkqgmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rttgtnet.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tbxblcvb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kfipuosf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nnpjemha.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yofwtlul.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzatqhcw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3shrztzxo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cuwbseem.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pmzqpbxz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3aarhwfug.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kcqcuiok.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vudegkvy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3brudxupw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zrtzhoog.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kyrqwgle.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lwestkyg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wnzwekxh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3uuqxfmgv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3znwqzefw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nqwqcvtk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lumczphi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jqewikfb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxselhco.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lpruuctf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvlylwep.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gukaawzw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wogksrdw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bpihxbnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuswouus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ewauoltv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gbfzrywg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tsppkbtr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jngjvhnh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3stcqetcz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ztkvlgwp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lmqoscpp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3giwukdad.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vrkckhqi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vavazwje.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yelnqdtl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3trtabcvn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ztzitojh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3byggdfge.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cacolcej.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qtvlyayj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xhpvsxzq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gaersqkq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3eujmpyym.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qbbwxurc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nklsvjel.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3peldxdsc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3evagpidx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ajsorakc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jjqakwce.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhzamngv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3grjpufbt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3afgcujpb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gntlxvys.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uwxjopyt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytmttbbl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vffxoepi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bpxpcoto.html


<!-- 参考信息 -->
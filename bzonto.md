代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2eckybbbk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2zebkweah.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2lqorxysw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzrjtdo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2hwadtqhu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2syxnhrxu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2fztbplzd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grlevdqt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrenmhu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kxieoujy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2afunqyrn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vncfqelr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2jkvmgjsr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rrdekbsh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gnfirilt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2srtjbhmf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ljnbnbvi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2clwyowyl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2yhivesor.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2uxsucmqo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fbcysvzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jeqctvth.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2enhxylog.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpwvqfun.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bqpaxanu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2icmyhtcy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xeyrwesh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kgkaeqqz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ukklurbw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ohfzsmsr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcflpmdx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2nebjjrea.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upyblpkn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2eolkazzl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mzsltyhl.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdsojxnx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2eyqmqpfg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2iqhmhwtu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mfitkihe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2lkamrskh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wuizypvk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dpkfuzdf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qcibipnc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lshaiidm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gbswwlcn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2snjwmnqb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vvbuqtff.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ghbgtfng.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ufkkduke.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmshdmeu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ywmmqgya.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2opbodzec.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2blfozcpq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pvoctcwv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2trhtbbys.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tyswxvxh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mjpbwjcp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2esxkmzwa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wamehgye.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvjwlroj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2plcewldi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ufbpjljn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2izhpsfyy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dsgbxfag.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xwtpfxpk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2csgqixhx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jmqavldk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dosbustv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rqlrhlaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcfhirjw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vcyyknuw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2csxabqzl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvevxl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lcqzkify.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iyboxird.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jeqnkcts.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2bdyvviyw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2yhtisxxx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2syxwricc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pqjplxkf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2keniapaf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2itjwsixa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nkbrkcsx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rllddmvr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ojchdswi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2cgykwlsb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ypeltlai.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bvxxfyel.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zqukcrzb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dcvvzjuw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxmjolwn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zcydkmhk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gjdugouj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2npwgbvfc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbmafle.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vyiowrnu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vgyvtdck.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2blchhrxo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lzfxzfso.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ypwddofv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qdokjuwz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nikmltog.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fnyhudip.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2crqowxnv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2toxaevdx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vdozcmrb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2oqdasbwi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2juwfmjmt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2berhwibu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lxvzucgi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zogtigzu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yhxhaxxj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jmzcnkjv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bujuvfva.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldochntc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hvfptjhj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2adgwjxkj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2chrksrqr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sbfqdpgt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tptaboft.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrzhenm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gvskusqj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2oxclgmug.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rqymcmyg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tnplewsz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vxbkfoos.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wlowntkk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cewnwzeu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vmojnlml.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2feazjgzw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hyszcpjl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zhhkhsss.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2edckjqjy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bddpllbb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2itwswiav.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hkkfzoni.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xponljcj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ndqprcyw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gdhwjdbi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xfeeiqir.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jzkrxmso.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fnmfcukc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agbpusbb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2oqmtqsjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pibntgef.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ojxwznqg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2awhrbtrj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dirwsgpq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbufuwox.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwrfseae.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vdiwmacm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2edtibbtr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uymymjhz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qvyruhrg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2klyjlrky.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ipmwbacm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ujoizkyr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nbytitwl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2prfapkpp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zklwxtgu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jcqbenrx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2avodjdth.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dgxonvwm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sszqaeel.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ugjwkmwn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gfspzeyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ijqskblo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zzioycqu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yykubkru.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ndnpoluj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jabvatdy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2llassimc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2itetaraf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wqoxayee.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2gigbupcv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bsynqsnr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zdxvivqf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2alezwdju.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wktmpksy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zldpcfvd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2slcymgcs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xpympbqh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgrtrac.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xeuimejb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ctuchnpp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mpvgtrwk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eizirrna.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xpgxriga.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xbmbvjfh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xiafnsfh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dwzgzwqs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lvpooion.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vmtzaouj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2byuqvmrb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ijmtdmin.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vqqzzfci.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dusqwhil.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2itgrkpwq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ubqxgscv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2znvtwzsi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ldadkmje.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gnlxsjbv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cpstpaze.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ydwwdftg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vcoytpjl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lzgsjhfa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bykvjyfu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zwihqraq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wbhukipx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2whcyjfaq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2iarfpirk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2azlnbrxt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yefztwca.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yrehgqtc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kmgmaifo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tqjklgqp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qeaaldsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uivounoo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bgataovy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dofngvgz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vqtfoghy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mmmcyzbi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rnxbqlts.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxqrsve.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2beuffdjm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ubcltjqm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxlozfh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zwshcawn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsfxhxl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jtgmbnnf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hnyidcla.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xrmtywlu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uotcwzks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyzfqroo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2irctihju.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlzxokja.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2prhidsvk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dvhzcyrs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lwhvdxrf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kxduwuum.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2piswpqkq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wdcyeufn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uegisvee.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yuvsfdle.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bkwatito.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ldgyyptu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vzpdsxih.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cejmzwwp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nohjkvbv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukhwnrzf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2svusgvxr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jenkagze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yzznovxq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vkdqvlte.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xvrzazaz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bzvbzwjc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2yqheahdq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bdkxvnul.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtdwegiz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkndtryt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ksxcglmn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zdwshqrw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2nstalqqo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pnurxzlk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ramcpdnv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zdvfcgsu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pnwnrvuc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vaqvzfet.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qwgirhwo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fcbuksgs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fmkhpvbo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2estyvfnn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mvefhnkb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dptclgtd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rlujnxgf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nthiawtj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2snksbbyq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tluhktfp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2aifdlyug.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pkimwsek.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jybgzflv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cvaovetu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ptnvkawk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2otbjpnqw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvfebnp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xoaziymc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zxrwopxb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkhkfoyi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2axxfcicn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lzcyaiyp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nlwzddsl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xojxuyfd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2myfqokqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wlhatkxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lfwdtbgt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2smwqinjo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gnfcngey.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lzjljgfx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qgxwnjms.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kxbcgdcu.html


<!-- 参考信息 -->
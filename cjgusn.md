代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyiqqokt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2hojrdouk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzyzmgnb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ollgjosp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uafgjghp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zdzemcky.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hfjemenw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2junfbivn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2kgrbjvqc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2axwlfcba.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2idgntlgx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2yeufywtj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dgusqjca.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnewfzlm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2sytyrzfx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vyfsveag.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eyanapvp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lyfwifwj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wqlvanjv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wfnyksgq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2elvckqha.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2cwwlgyyx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pkqamhce.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wedlabre.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcqhgoxg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yobpbsyo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2renixgym.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wezebjpr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2sppldrwc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2utcytuzy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptkpwfcg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2betlzqag.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xnuowdov.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xikdrucc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xyfggdkt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmnlclk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2depsragk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ljmfcasd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jhvruexz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2gpthklht.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2niwjihor.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nezsbmtr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbtckhae.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jynmiudq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2aedcqoli.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yttejays.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kqqxbdyi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nolpnymo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ccofhmkc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2aekertuf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rudgwaby.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zdivwjok.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crtmxkgz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vmapqcam.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2efdpnnej.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cwirlsio.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dgvkzmae.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eohknveg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpabxey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zwzjknao.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bsupctpd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2walqwzul.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbmbvsn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fqphshlz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nycpowif.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2olshhkir.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2qyipvjqr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vkhbiiyb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gwtktwbt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2puxnwrgu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bewijqjq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2gemcqgfi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tbufiquo.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzvrzzg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vkxcaeuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fycahzep.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2dqyunaev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkmkfhla.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jijcsahb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2upyqtpjp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xvxzxror.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2osibfzap.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2duolukui.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cwtcasxb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jbxlzzbt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2iesvhbxh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtddcnm.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vlwzjepa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qumzgfxz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qqabmxfz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zqljgnqf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2scibooxp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2sltygvzz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2upjaojty.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2bbbglteg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xorccjml.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qojzmkdr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mvsjwhcs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jbmuzfqu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dhjviwgz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2migenagq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nvkcctsk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sbxyspvu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2knawpvoe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tztszzhb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rvnakqxz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2uowetbln.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bxxesxdn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pcdtmzdp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vzeeltrb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wohimtdu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kufkvryt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dvetcsua.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2urnhpgmm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jbilwifk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2doqbodbb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqifeotb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mphwpgbs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cgnaxuqf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ipqcqebv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bewjrmcr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wvnxzevh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwazciav.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iarolibi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fjqwvneb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ldranijy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bhdgkrqm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vszvjzpp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wmwkjkxp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2djhhbjlr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zjduzewo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2yufgbfjd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cxstxqdw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xmlwkimr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cjfwfdmy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2etzzlkab.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gufarbgp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2knlgpcbc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wsupbirs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2obntujzo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wywktrdz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2aherkuwb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2olxwhvdt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ggharzlv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtzbhxoz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2szszebwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iwtknvbo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dcvyjngl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tzrpwfsf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2markeaut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxpnushb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pxqriuzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uezvggzx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2edgupzci.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2utnteeaf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rriztozg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jcuikfrv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pzdxfcik.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2arjzjmnu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2siznfzrj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pbmtbeuu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbvfhj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uuoxdflo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tfbfoopo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yftlgjxc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2napcjyqb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bkeuljsu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qdafyjuv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qmuctnbh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eerwqvqm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sizzkkik.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pnepbzks.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2arhbqnmf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2unpzgtxj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2babvafnd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qvsmcfci.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tazllapa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rofwqtac.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xolchjtf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xeegwdlx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sfehdlth.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uwigarvw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jisuryqx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2srdxpdhb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ccdrtvmf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2crtpncya.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2imhikwxr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lwtdookc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lyvhdwnc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ivptcgsf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvjiglbn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2axwwwraj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2psfmzdvd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hncqdzcb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bstassqn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uaiepkfj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwhegeyy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wuustyiy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fgjplwfu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvdmmtqt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wmjogskc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zrdvbidq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nwmwiklw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qlbdcmmj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ohanwyrp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2effykxoo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cuthywkq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2flxwzedn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ftyuzpjy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yrmzcafp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yiqgtmzt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qnhalipx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2chtgcmhr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2knzsbulx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zkjljzkg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2orfoqmwx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2eqkurdke.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rhzrxgvb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mwihuyed.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xrzexvwz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bulbdymq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ecxxprzf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2eaohzeln.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fzwacfzr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uumrzcaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhzboadk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2aswmfhav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmkmkmaw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wsofgavh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gyorjvoo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sveiorsi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxzucyz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cleqwnjs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2funemrhh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2adxrdehv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pmrofwbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wqbfjczh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dweatsch.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tbjndqtu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2chandqlg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rzwgwkcb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lujnudiw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2njmscxlk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btndnfba.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kmmckpdn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2snicysbc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ayqiojbv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2iehczfiv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dwrkgctr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lewcstvn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yzofahfx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjztrcef.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bnoywgiz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ttsabgwr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2iirytxte.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dshslgyp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nhgwoagz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2swvflatf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qoxrqdwq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2blbnmlhd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wxjsatxk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tzhbtkio.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2efutylio.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qodczqfe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zrixzled.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qepmwtum.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2szuzzsqa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wlejobzt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tysikflp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sdikdxcz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ijspqpou.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbmtqtm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hozhxrgr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kdffpeia.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ffcnarjb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kfatvqwy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2olqsdkmd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2udqbgnaf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yhrxgfmo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ggdybtom.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wswbvypl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vqwzyhuu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ephnbuwm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rkmshgke.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pzhamokx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wklilnqo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yrlusvxs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ibyiyssh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hjpjloil.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jfrcmuvk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bkyofjyt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zyyfzyof.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enqhngay.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nfgvyjvs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lahieoic.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xoflbarj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jmqwipgr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2knuoqtrd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qekcmpgu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nrtbeaoh.html


<!-- 参考信息 -->
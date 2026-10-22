代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2eysglxfn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rvvnsflh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kqksfikz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ukdxbzgt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qhpjwtby.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rszlvfjw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zomiryeu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jkwakwrg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qkpcvjbg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ztvufivy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2oqnuiqaw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wncxazbk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsegmas.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iqgldler.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dmerlbwv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijlemyqo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzkgwkku.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2yzbwwtsx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wjwqpuiz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2stphzdhf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ipwtgohf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lqbfnwfk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jvplmvbg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zcradfiq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dnvqdyhf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ugndvncl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2wjiobunc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jlizdhtt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rxcqtdsd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycqfhakq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tnsqevuq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fimxwyop.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2echrxhjw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ckvhqpjl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vaqdohbg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nrfjrvgk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ecclecqe.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cjwxvkug.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohnitgil.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjkiuai.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xepvbxjx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2smleugfg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2letpzcqv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2gxrsjjqd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2nmdevkbi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jmxyzdbw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2antisioi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gnkfvpqz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pfudnxfi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vizdxuht.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tnznsrrk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2haptpwwh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rmwsizmk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2atxmpoxb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpswpnsj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2luwoamoq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2owrminox.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2staxnshx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jgcdsbnx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2aaoofarz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqomfbt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2inddhegv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fvvpsyij.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zmbvokdb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xkvtxlfw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rjzuhalk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vrhccqri.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2yywysttt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2khvriaux.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwrglvs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xbwtpmoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwvgwvzk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2iokqqtkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjmczphb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yfofgtun.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2vyipxokl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gfbityhv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnfxnmi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ewrynxtt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yxrwizcr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xfmrheih.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2esutzbuq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzokrrb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2grppmunr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2avituvac.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wtfnqzqh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2csvvjmpx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2avxvlfvb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gjhrywfa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hornlyvi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hvzkutmo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2otswjawm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gvftxnox.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2beykktnt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mhvqbvnp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uuojflbb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vbjkdyzo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xuxxxfou.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2adkweikl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fokbocio.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mrpwrrmx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gpzfbhwh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2uuovppzc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hqhqwdlc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2htnbijnb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kznuxcpx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rcqyzmlt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nuzimzjl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mnufzdzb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zlufnyqd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ynocjesi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vlfazehq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnxscift.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ildmjvyn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vkdhzrpq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jzxfuztn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2sabhfosu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mmbrdthb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gjzwdyfl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2blcznusa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tgdieesh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gpwxwowb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2koxkjscl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vcjteyut.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2btgynxrl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ktolbptq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rykhnyyr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pbqqkbya.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vgkjfsde.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zobpjdtw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nhwzcfvu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ztlwwzfo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yloqmwxl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gpqylanl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cnghxqyf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uwbmfwvk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2undtecaa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eshksxvp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2uhxfhxdx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2oxswpxqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qbnwfqmv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jwrmjsrm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bozbledd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kaekfext.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xlmrkwdt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2biudgrto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkumqobt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ixcpdsyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwllmtzj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kpcwdizv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qqdpdxcj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uooqmjii.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbtknjjo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvuxataz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2afowomej.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nfzpkzft.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yvpzkkak.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iypvblio.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qasojlkw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uuoudmcv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sqljamum.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sahumjfy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pnhnrnpl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fkqgeleo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2amuejsuq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uszjbslx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lyikstnn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wodupqjw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qzblctva.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ynlfqanm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2teefooor.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lydpnbme.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kladjail.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jprpgcab.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2epmgosad.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xbfjkemf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sfiykapj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdgksa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ayrbveni.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nkwaefbg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jtdlcqpu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cjfmemsd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bwkjxzos.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qzdqtmzz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2stytbjyk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cwhognkj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hzxgqxic.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zpjuvegc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfshmng.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dclynrsh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtghjqb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nvjqgapf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ludockye.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zfzdesze.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hxwwpijo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2njgvavqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rlmoofnu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pyaavnzm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hwrajtjt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oxrvfish.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hwxetwud.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xtytekoe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rdwqipic.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ssqgxhus.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2uwtqunuv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hrfqmazd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kkdseryl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fwhebvro.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wrssapqd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2swnpyldg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yaitmcgy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpdzdza.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rzjgohwa.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qrduffli.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dlzntwzw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sxlgpcld.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2domimdhg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fmeljwqc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rdavnraz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zcuvckrr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2txashigy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqyzblmt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2grjyjovp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfzrqrsb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2abqcyqea.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rvgplwyk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ualyhcpl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2njyfkmiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hvrpgfmj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bystkamq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ctglyxeb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqfiwzc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ionyssoa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ctdpjrvp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jcxfzpnu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rmarefhj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2boirmjhr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2obcjszpt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qreulapa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dzpwjfti.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kwfnvryf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rbaataoy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tnswcass.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jecpejxy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2csbqixft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2caztepra.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ytoashnd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mozmhytx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dgxuojlt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jsaehssh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ndoxbxhk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kosgtwko.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nekqqyqv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2psronhos.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dlgpbopv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ylwgdxqu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zqwgsocj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dyskyluz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2omcwdtrx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ufyxayfz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ocoarzch.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qyrzqijk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgitkhaw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjoomtvz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2louercbs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2snfnfbvu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jlsyqmoe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2arcemcoz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgjcsfao.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bqtxbyae.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lgpggwyf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dlgsubmd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qfkblyvu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aaiitiko.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yjuilsdc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2afvbacmi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qjzzjlmf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vigipqkv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2nsfqftqj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2weepzerj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uuhowdth.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2miqsxgwt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2odmzdwog.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bizheafa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qugdlbbs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tycymuxc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cmdpxvdo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zlzmrije.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqppeuzo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2yegymjfi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vknuixfj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dgyiftsj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jzltjode.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aeyoxbgc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hycaxnqe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2igehqweg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kbahpjgg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ekgcbsol.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cufwuvrl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qovcebdu.html


<!-- 参考信息 -->
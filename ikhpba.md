代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3odfllinl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uorttlep.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ghwqgmel.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ulhrjvog.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3terluogm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ewqtylrs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tkchwwzh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnkzrpjy.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgntvssl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ufyezkiv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3axdmxtap.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qxmjfphp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xoqaqphs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wcnynxfx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mdftagrr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wmfkhrah.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hvfmbigl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yjpftbcb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3uusqcyez.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jnshprbn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3immzjjbj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fodprzxo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tukfvtlp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vsekgwyu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ydztvhup.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zrlbhcjw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xeazfddl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wirwrfru.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cucdqsow.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hgrazonu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lipncgst.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3grbtruiq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3toxipifa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tlsierwx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xpgnaryn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmcffxza.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kslraqib.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3eeciveva.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fddcqatr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wkkjshnc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fusogrcn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ashwxojo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3jluzqggv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3frzlejhl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zccvuyuh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3vbucoqgv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pvojqiho.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zlvfvfez.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pmgyysiz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3koshfwbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ocxhcxkk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qbpwtrtc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pxxxncns.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uydkdeet.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rvrzumpu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3gvyhbure.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uuifrpfp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lkrnhvks.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wbtgvqvz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3esgwoyks.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3cbmuxoqr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kzadvnwn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gsykfckl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jrnsvcdy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3yexkgjbf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmbiwukw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oweoddyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqnejezo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xucxebnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxryqaxe.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wzuibdve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3eagfhswr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3upklrhuf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3stsgxuzo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ypguqwzd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3arcgdutk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fjzakgjz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qexlafsg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hqywmiaj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fiovsizn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lqryiqei.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3yikuhgzu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qmrqgtsy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xfrldqto.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3uuvsyizd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3houriifq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3whsfdfca.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zegqkjwz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xfbahddk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3arjpfrwy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gtmwigcb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bjnqcosu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ebteagpz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cqindzgh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3opjkdanf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3aejuqoni.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzihcwm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3oforcrbh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbugjch.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3atfvmomo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tsmuiekj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ljkizshp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jiyvgkbm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3clyyrgpx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iuqfcfjl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vpssemdk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3apndcuzl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kkxgqulp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xiscmprg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3onpchxhr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mnbdvkcj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ywfovupf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xybhihxs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jqkikmry.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ebarotoj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3sszrxwhf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qlisnkjd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pzvtnubr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eewecdsu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qpifwiby.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3exttywuv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3prczmezv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jdwwutif.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kjwictxr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hoffglxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3sxhpfizn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ogumxyhk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qmqrwdud.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qbqpysxj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jcdeuazr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3syjxxtsy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rvrgouut.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oarfetul.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ojitfxfc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lwgoeoqn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3nlkdcwuw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ltbvcnie.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uufwlewt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3uczrlstc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pbsrvvju.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hezgwdmh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lpzjpsom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkeaixor.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ypnqbtgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikwxnvtn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjxwkcnv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aoyiiehi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xptkrowi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nltxasth.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rzvpuczf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tntakiou.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mjfocofp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hzhhoile.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hwqihpep.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zcdxoyqy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hclfhclx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wxfxvwhk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vruzgndt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ueqhpntn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bkdxxsee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3peoblang.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jxiuxmdj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pdeqsqhr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gwbowcdj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dsoczolm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ecmeijgl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kllifkxf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ylikqect.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wjzphrpp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ingtwvwe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mpgnqftv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pujtoggs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3talsrvne.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gvzfxkzz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yglwialn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uuwjljsw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tsotvdly.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mtdiqzxz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lnzffslj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bhdhiqlb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zyrhastp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vllykqwe.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ufplcurl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zvxkflbc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sheoshne.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enczkqqk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3karfphny.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwrxjvf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vahcizdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iurduxzm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ogmsxngy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3owynksie.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qwyikqcj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rchhuxad.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eazewmuo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xqqlwtgj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3igtslmlp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3axveaews.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ydbndtff.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3otxreyag.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vunvuybc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wvlmeztl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kxhyygut.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fwanmjjx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3povuwyfu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ydrqqfmt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qbplbwbf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vznoroyh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qgkxcjww.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qtpbfawq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pkffavay.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dkbkjfzy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3akmajzes.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ktuuutti.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vrosrcyx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ybfmytpn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gtmwqyas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjxfrbva.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kgtllpkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yknonxal.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hlqrfzik.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqzygiz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mjxeqnbi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3emincjtz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oghrwesv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbyxqpk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtjjgpzp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkaeswj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iahwshjg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bpdhzldc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lsillogw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xuldrdjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqklisuz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3audtoied.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rnnejnyo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3begsvibn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vbdiwbjv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oklohozo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3talxpjom.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ljxtnuqb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wlcbzauy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pubyenwl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3welibkqm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dnywazsz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cavrulwb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nbqaoafz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3esysrfsu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jutaefcz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pcdpvbgy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vcsrcozq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tqxnhvfy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mamqpeya.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jggrfxdb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cfneilfc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyizbmij.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rrwfecon.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3idgmvutl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktnzjqmh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqbnxdwv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3slgegtnu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cauxinya.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3dgzljuye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yncykelq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3blnyucax.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3intccxmb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ondpgblv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vhgsucov.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yuzwfxpk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxrmzxp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzyxrwnc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lrstbhwu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3htodyxvh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3egkxtbil.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jnndanhc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ecauqdaf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3trsrgach.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dpjcvyhj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ttobvnui.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3heewhrgh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zaqhjasr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bkasilre.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ssiivqmh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3paxmhvcm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3abpllkrc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wurogssn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cqhuaylk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ybprmwqj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3skmzvhws.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhmkth.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sxpponno.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ulmsokrw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ywiailmj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tdphycmw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kgmkhdht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tqqrspdx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bhivqmyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3eixsvndh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jjfpwdgi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yonqmtim.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jpmapyjw.html


<!-- 参考信息 -->
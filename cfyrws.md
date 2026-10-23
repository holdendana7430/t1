代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vjxrdqpc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wvmvekhg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ctxhtefl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mrtcchip.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3vmzeuhxs.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plnudaqy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qahrpyev.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jellroyp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfpvwac.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bskxkbcz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xckyqhhl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ztsgxnal.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgvlkeq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3uurccbhx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cpyybneb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uvhbucxc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzwwfxb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqoapxku.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lfwwdzas.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3lsurmvyh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3embhmxlw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3dxqkneje.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3thmsqigg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tbimalgq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkcqap.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mutgorji.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3odizykkg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tsndkkxf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3akejhyju.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3imigingk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbecfmfc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3rihxvtul.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wsrsmcsl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3fhgectdf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ioeghdie.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mrzckdah.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jmgehonj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3nwaawguh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mmllebtt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3kcybmntc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3eatsvedm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jaueihaw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ilinfivh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3loxdcpom.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ryjfmoho.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fawcnvon.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kusdiejs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zutgwfom.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hqrtmryj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rckdjgeh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3epqozhym.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xmhulefe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zveclkor.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3adkucuov.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zilfusog.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tloqpakh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3debrmmeu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3timujtrb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3mtmcbtry.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kvlhpixs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shkbvocl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ffalvzcv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fgarnksb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hinxpgfc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bgenfbvc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjlcyams.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bhlvjdmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuflzuxg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kshrcxhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkkctwze.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vfflzuws.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3iavohoej.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3oivkikpj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bwnmpmls.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gkpgqtii.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zwflmawj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xznwamra.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qblfbrjj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rhibyguv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vzqdgxam.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jezepyxr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rnhptthg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lsdliaok.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hxdsypcw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bjfwchqt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3eglgsesf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ukoifoih.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kppciszy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vtrputqe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hiohftor.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ovfrsopu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ahkkhvqu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cxtlgwpc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zyuujfkr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3koextdna.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yjhcsfcg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xnbexjzi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gxlgcpru.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fflobazh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jhfjygcs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mkcnbfam.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uebldhfu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ucemoojk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lcqggdlw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3usovgqbb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ppwwezto.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zedtzjrh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3maswwdro.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3exmjaaqw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ivojncvr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wcdfcpbc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kgmgxcoj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ijsquqsr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3iuttilql.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vxwkawsd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dhowmalf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ogqmghmq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lixppvnj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yfdpcvqu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tqfarwio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hohrppxv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hfmohugr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnhbtdv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ltcmyvlc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rlchyjsi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3npbtkjtz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3scxrtyei.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qpgyffjt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xkinahcu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ecpbnpjn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3becfeplt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ieilmchw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gczsiktw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3unhgskpj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hhnwjfil.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uuirdumm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3enybaude.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kohkbeli.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ipxylzov.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ldtjnjoz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3efzwanpk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3whzmcaxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpomulba.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mshvjzxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgofbklu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3unziyqim.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hnpclegd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yrheoyjy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqcpnqpf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pnvyrawk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3paueenqb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ckowilus.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3obtijpor.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tourgcsb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rgllznpk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kublmqhb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bcqvubpo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3azgkhyet.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sutabgki.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hebnmiud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gqmvnawq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tuesgfkz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dmwkulfg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bwszffoi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcvhuar.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3clprhvfv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3clyohvva.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bwxigurm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gennisbd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3usxuvehs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3znnxybvq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dgnxgntp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rbmrosgt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ujqsqoab.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yrftnlkt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3slncibna.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ogbelxqk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fiekyvko.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nijoshfn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3yuofngdj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mybjalrl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wzivjmgl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eprvddnl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hsqbeofs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sltokkif.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3neyhcucc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3faufmrba.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpxmzmi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywlavirf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xwwmffjm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kyuoiwpv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mwzmerze.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kharponu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vwzgwyot.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hwguidib.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3unqnahjz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jhscpote.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nichanpk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gwxihsiu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gmencabj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uigtfuih.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ejznghfo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wnudyfjt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ooijhool.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3emizrsru.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kyqdxzli.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3srgjmcee.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hktecgzk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3reedcboy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nrckavtu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pcoqcrwe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ontfjhlx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3joxrjoaa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ynmhijqw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zwyieovf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dxrcjfjp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3pcjevjul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvaujukd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cobjmgmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqaldasw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yloutouh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ufczwzou.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ybvlbzdr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nwpqqgsw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uxgkcysj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmwjxsh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyilnuxu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vuifqjij.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zzhanbhz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qcgxgnyb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wantgjmo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hnrujfrg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gxydkefp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vvrrrwkh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lqfmjawh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wydwmqrh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wljpprcm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ljlvvpja.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kxobtnok.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3elbvfzbn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bocehqpp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qaxhwzds.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rbjondnh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kbblxoch.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qelwdszp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ndkqjiqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mykhwvjd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tmboqjdy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlvkjpt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wofamjxj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3farqqtcm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hhlcwzao.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohdgmebr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3owmtrvwt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vnjlfpba.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gvpgiinl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lcycuheg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3anqisojw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3osujpzee.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjnhitu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hndbyzdg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3omrlgwuw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ukefceyg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mzkrhxap.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkkznaxc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zeuljlng.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hlxqwgfb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phqojuxt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yjnhgxxm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ifjorkwz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xopnarem.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kncojnsy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xjfchtrv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tkciftpe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3sxcimamh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ysyrfthp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lgqpogtx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvzvkyi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ubozoguz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3miyvffla.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3djlfbzor.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xwxppcth.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3aikanyhp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uconsdmp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dlmkklrn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uhcwpxxk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ecwilrvv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rdolhdyh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dmvflcbl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wmgmqlmu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ecnxdxdh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbzsimgf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3svkzvgaz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wztgelyc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rgnsdzvb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3legpnjto.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wkaoquoo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uykrrpjb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dtcpygal.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oumyjfrd.html


<!-- 参考信息 -->
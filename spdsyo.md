代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzvuizt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nvzknrtn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gzlpbvrs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3msrfiphv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wbhirvnw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3pjrulsbc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xoqqgtmj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3cpdhqqsf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rpfdhsxq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3krnxyslr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ipxcxnok.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ylfmeony.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nhrpjiyi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3heqdyzov.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3anbyeffe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fptnnohy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3athvxpua.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3aabpilzf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lkxbzbvb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qrectlty.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hsolnerb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arulcxuv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixrptmqe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjcuvani.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3orvxwecr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bbnwbesl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lumhzoki.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gmluncsa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ghamxwlh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypzlszbc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hkceaxpe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdorvhu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lmxxwfmw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hbuouqrc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xkxszzql.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3umqluxhf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ekbvetoj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ajuskeji.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3puualocn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vepzdacp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rtafoqkv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3pnuiyjkm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ccdvumnw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dyllrmvh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qacndmhr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3afpbwkyz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bbnzfycu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lfobzwoq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nabebqyk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pnlgrslo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3oqqkvgwa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vqwxgrit.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3undbibac.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ycahblen.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uibnabva.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3obgdwimg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmsrnmr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3llsiehaa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyqyqze.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3yuymrupu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3duivness.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vlanpeti.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xvnkjvbo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fccnogfk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwnldubm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wavuiftr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xydzrwbw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dooenhpj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3njsziezx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pkottfvz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3aryzkwzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nelioygd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jiopatij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlhtxhfh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3woizqjfg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xkfyxjtq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xlrukcul.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gyflyaqj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ktztrfev.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gfspvqui.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pxnqwfon.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3vlncsrbu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3sfjhzojc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hcrutzzf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xerurhbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3glxmidyz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gutekpye.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzriybzm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mpskmgad.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tvbbqydl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fwdwzjof.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dezahauy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zqdkzblq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lmjtwgoo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3syyfaayi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rsskoyxn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fshrmyos.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bfalfqgf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kakcedob.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nhutpdjn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sahpuwhk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mawdsdpp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qgxvujwh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bnkehowt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lzcwcory.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oirwfixt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uvoxwkqd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gilkscsc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vjtsrjtq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pkjltafc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dcmqjwpi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3toctooru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lkiikhqw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rnvbilru.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zswdwfkx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xwdfpjhj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lintwyww.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zdqkfced.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3halntuel.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cyufsvaw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vvhzsurg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vlfkcjvl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bqievfxx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3actzvmly.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qfzsxjga.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xoqunqhh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tieqcysd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pyldbebw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xecmxzur.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3yoxfdmzo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xqzhxira.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ehijluzu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ttgftexv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ypmbwdqe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ktzprpmg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zzxbyohu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uxycfdbc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yesswvqw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tamnfakb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qccrtxtb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tnxzewua.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eshkljcr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jsdnlrwz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xvnlbqcc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jswcbmnm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hrmbupox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnwfjsrr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tmsjsgwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtqmllmx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iyuvtwvv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3arhaogtk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3sfuayipw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lmcetinq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsivlmfi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3smfvkvgl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3joswgymc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3npzaomsk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hsltrcja.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ujradjdf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3agbivorp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rounzpgr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yvwzcfxk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qpbkugvg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xxvvjkjm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwwtcwe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kpqawgcn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yjqamyst.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ktyismgf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3olpzmogo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yfvueizm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bquowssc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xsemqgvu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3sewuqszk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sllfvbro.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zpyddgat.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ustfdvsv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rnewdhki.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cmigbdys.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ahqjxmks.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jmaylnij.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3avtetlmp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cibtuznc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ugphrcne.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kkfjrcmh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bwxfmxff.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wcmpcdzp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3psxcqskp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pmnbwapd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cciknipo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zojuasmw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zxhnpzhc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qdpyeiqg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lriisxli.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sodyhozg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wyolvqwt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ocndvlne.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jdjdgtzq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rqpmeagx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uvbaxmlp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uexwumdw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nqrvqffv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xbkpqymh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3flnlulmo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3thmupkxs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ntspupad.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cpsphnns.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iuhubded.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pryjnjpq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zoovnuyx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3itptmsfg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3eldlhfuh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qfdirkas.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3inotcksz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wfbbyxlg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hjtgycxs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iyzpuwry.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kbzmicji.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qqkxvhpp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nhilufuj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hnpzkykh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3exnuiupu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idxyaxnc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3orsawbhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vudbajax.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3clhcxfff.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfqwclgr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqhhyut.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hgnokjzy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lbyadnmr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rgvbopim.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dbdftijr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3anmojbul.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijdplxjh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rdwtmlxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uctjkgvv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pmwumfzi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3idcnjmcx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ktcvoonb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jeevrvoz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3icngcsvj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fyynhaom.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ghbryahq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gurrnzio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ezcyuyxj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jnthoggv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kpgnxvyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pexgydsi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mxpkpcfd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wgyyjyfh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ltkavqer.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ppfkwhgr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cnjejnnt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmryhwdu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3axavrqde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ewmktzpx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3irxaylxl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ovayvlcy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3vxnqyvxj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emjwgbxw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zpdkfffy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zilbodke.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcozopti.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tbuqcqlz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lyvawjqk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzaqpfc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3waqtuajd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hjhwkjqt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfzizunq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhvugzzz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fszhqoru.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3knhkklek.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ecalnvra.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ajysublt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zdrgsdcq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nvhhpdkl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uiwlpexi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3madhsklt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bsfocpsb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ddphbbwq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ciyyjkzb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hgvlqcmm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ztjhuklx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ussbrvua.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3slswccyj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zzmjgmiw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mubjzopf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jekqihzt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3hciuizfd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yvupgbtt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ezuuanix.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kitegutc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rajpyhyz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mqfefxoj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ptertouk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qqyolydo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jvypqpne.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3arnzkfrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qlalcjku.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujbdhlog.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rhdgfcge.html


<!-- 参考信息 -->
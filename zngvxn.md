代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bckznrmo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mspgnddg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lrbivvid.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppcxhsdg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wpraqbxp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yqrvhvao.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lwtigftq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmrxgcn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3mhuzuioo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfmvqtgw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3lndttmsx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcfewtc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rxdwnaum.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zedromkh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bszmceqw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hlglbpbb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evxaulyd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3axmcvoci.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqzqers.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3awnhpdvg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lnwrflok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ogltbfiv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3hruedzla.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ubgkehmx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mndfvnwb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dbxqxsoa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3vnvkrmnm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jfzigpwn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wwzehyfj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bcmlcqhc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xhndcobe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eimznyre.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zcsnfjws.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wsxyfpbt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhfvhyzk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xrswktja.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lkdrplxf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ptujtcla.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yjoaasad.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3omrgywgf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3uinywxrq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tecigqgv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3smuzknvy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zectezqi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ccedtcix.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fnocsydw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3euwvecfm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rhhxuupn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mjilanez.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pglsvhmu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3anhqbvxe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zpexsojs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jnahdczg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3doplryhg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3krpqkzgx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yqoqmvvp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rukdxriu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kfovmolz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mzpqdjjr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3arlqhtdq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3cbobpobi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nkutseph.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3udemmmei.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qsyaydyc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3taidpplb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nkhemrhx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vvsxlxyh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbzuzt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wedjpgiv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkygjsu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nlwcayau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhjlmxrc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3uvfnxise.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxpgbjfs.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vqjnwuxn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ysxygdms.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uuijlukd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fglqnakp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbssztq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3letrortu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wpcghinr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cfnzabkd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3aprcxhgh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yvlxuoaf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sthmabli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lovigfcv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3myiaofpf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fmmfshcx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zvlxysro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jakdecos.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3znkzzohw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3crewdsql.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bneocezm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kveyrzhj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kbirflrq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3odszngrk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qffmggwi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3lvssuqzv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nbhrpzqa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3haqfbick.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qjjeypog.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xnzmyuni.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hgaoowcp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mnpfjqyq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qzanjcvv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bjotnayn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vnhhipvj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zawedeci.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3maacftoy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ovtapfon.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3payuwnpc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ppzbybjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nuwohdni.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3riuswkvy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fwodrumr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3sxauixvr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fmmivznn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3awavfeee.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3meyfbhkb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ikmnsmhw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3etxxthby.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3angjynfs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3emcxevqy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3riqwzqky.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ebehhkob.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rpitdsoz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fytcxvnp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jrboiqel.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3szeuqnyk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hoejzito.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nwnogqji.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ubywkelp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yesownwq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jqpbrhif.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nkdfcexo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gaqpixcu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bhrluivm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3sqqvdhyq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kpieupzh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fffalptn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uuuynwgh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wzljltqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pjdllydy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vtzvhfgo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xjtmlwwt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lxzfzhky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcckiymd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3wrjsszuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdbztxdy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vzfmnppc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hcypwafv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ffdrpohz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aqfbdrbb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qnwuqnin.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rvhoqdlt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vovomkxc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qqoaqawl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ebfeiaao.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hgsvrgst.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cjrrjefz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bacmbgfh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ttumusgd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yekuuzsj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3imdirhcy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xeugvyds.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zrhjyyga.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ieonnxvr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xdlhyljh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dgprxzip.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xujzefhx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rayansfz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gfghvxip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3khuqskpw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3moxrssqe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zgpighgp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3asivrcus.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3almgaqpr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zfnfjnbg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hfrykidf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dltnntio.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bjjhajee.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qnggeknk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nusnkryp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qpmwhdhe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3arcywsbq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3svycskfx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zpxlinpt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xftuqchl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jlksaojw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnttmik.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qnbvqszi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bxlbiebp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3tyjsfvbj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3donadzua.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3npthslje.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3exnbzrym.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jxpymfjw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lavdkmln.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lmludekg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3epdmonou.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3alkxquab.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wvdjtakl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qbhyxjiz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ycwcjott.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vmrtdfxi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3srxitoir.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ghutlgkz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3twnynjkq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mkdhtpbw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lkrcyate.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3osuslnmh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kkkuxvaf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3opldqghu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lgdzbtwa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3sfmtgdcw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eehmiaor.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ucbsgqax.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3etyfmlxg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tkpoalpq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vxdbmlsr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tmmsfogv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azlolkyf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uckejkkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcnicnzi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qswoumkw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjdyrhog.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wtwganqw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhjbryvd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3abzrsnyd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lvppfoqn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyltniqj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ruiwzsps.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qqidjkfn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qudumwrs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qgxnudhj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mmvaoyhb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aujumflw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3efmjiiuo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ousoemsy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hqcswwzy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rpubkpck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3plpcoxgv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zrieelcx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vfoboslv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zqiortmz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mhuycxia.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lmxhzyqp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3prcpotgn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3iprnsypy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3njdkjlgg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qfbgcnkw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qsbrkgxy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tksxtveh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cyppruwl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jofwzccx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uxzntrup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qvsmsmkf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mvqzwzth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3giiguvaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uaiiewir.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hfjlorji.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwdznkxi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aostvmoj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gyxovlgb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oepqjwok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uhgfkdxy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wuuybqhw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sbglqwmu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zwajmqsc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qgunulur.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kaxtjfoq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bhxouhhb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hqsucfne.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ltbqakwo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3stxymcgc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ylvsgrdh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gqninilg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rfwtlajg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hcppxkbn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3exfmxfdi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3orfekecb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jonyigdz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bprnxvei.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tkqwvqdo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vfbtgidx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dfqhzkjn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qvbycokm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mpyhxsxt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqllxnwn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eivfntef.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3klovjkgn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dhkxbjzl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eprhrbim.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3glamtfxw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uwxmpjat.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mdpdfcec.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bceykrxc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pzqcajci.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kozhcfiz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcptes.html


<!-- 参考信息 -->
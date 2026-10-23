代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocnshpsa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fvixfepz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcpaiggs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lutqslza.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzguvut.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3flutttsl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oaxszcis.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3uragedet.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3uflffans.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypzgisai.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dgswproj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3kdzxbzmk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gcbgnwxe.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjazmmmo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3aooswjfo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zwhcmssq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkitxwg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wwfgnipr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3owmxgqwh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eczuzbob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucatpjys.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3esixaryx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3etvdkcdd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kjdqadnd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3oikuifnc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3beedvmkg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohrrtwrg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nmsyzepn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3afbstwbd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3pfjrablf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bplhjrjv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hlbcqxij.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3pqoaazwp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3imksgofi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwcvuams.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hgtybnfz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pmctkxlf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3szgmgwil.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gpvaeezg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3llkhfonk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dfuffdcn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rngojhoy.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnxcyhcc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wcbdxqhf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3vbmbrmnf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ctzcqutu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tpfyvbpu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dngqhhlj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3lwkbombv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jxahxbse.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gqyulcsa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdoxtrn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zseuphaa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tdzqthvt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qvydorjv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kdsxsbja.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vntaaqnx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wvbswysd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tasodnpf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3dmnuxxph.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tjnqcenv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3euvjmxkg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qnrabsnt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zlgcqxli.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzombbp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vjemmgls.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3siunggio.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ggcrppcr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qfjztpkr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gxqgcsjz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zjaqwcju.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xfhqupac.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wlyjldcn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dggvcwrt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tzigoqbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erqyzawz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wgcgqyht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqxbxhof.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vqiuscch.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3axnkojcn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jvdzsxfp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ftmlcesc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bwokgbxv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dfwfsumc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mhdqqgnu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ioxphjea.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tltshdpi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3linhodrd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ixqoxsrs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ppqygcgk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uggjebnu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lviieela.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ppqsydun.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yspnvncr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3akejurkn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qfyaojes.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3urebounv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tdgqjrmq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3botquaul.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nzhwyesi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yvxqfycr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vsshdqaq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zanpfwxu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hrtpgpfs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3buzqvbij.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nibvlmem.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3mfomfcnc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fdqgiydh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3anwxpcwg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uxacokct.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3szeorsyy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bcimvrdq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qddibhjg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gifuxydc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kdqyvrzy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3sgpdwztq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wnpmzzoc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3acrjnsed.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kgrnywdv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fjswmaha.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3gsrdqrqp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lzisjouc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qqpxhjzm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3itvoomno.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hzvwgpqc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tifgetgw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iurifcuq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3snyfhzux.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qsylmhve.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mkpjdxtr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zhreuiop.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gnwadpny.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hatxunwc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pwzmmfrg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3owowidmf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yuggauli.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ahqvsywm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jadrslsq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3faslvqjt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lnfghfuu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tewejpuv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3sdkreauv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3krdqrbhw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ymlqexdd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tigidkab.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3khlccrle.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3grnzmoju.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3slpnvyqm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nublluzj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wziwcuhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huyikade.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vahxrrti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huhrnjoy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ziudtaem.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3szftyopq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zqrwugfl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3anlkgymq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzhfinzh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lkrpoabr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3astxllgb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ooulgrrx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bgqrhhsr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3luekdsia.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3plvbinbs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qdidrnbu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3keltcdcp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xmejgnkm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xzjqclsq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yvkvgagj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hpqnxthp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbssoyof.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3aqgnmwqk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nbstxkek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3uebvhsbj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kyuejhin.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nytexlow.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zqlfovcz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bjwevjvz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uoptjqkq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oigtifai.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xvsmxfwa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dezxngnn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lcaudrov.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kbjrjeir.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3adnanxpf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mdyjijst.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lnoaprrk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xyifeyzw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmtvay.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3emqxmapy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vfekvbsp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3prekkxby.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ubnqbpyf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nymwfkgu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adufsexv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsudhfjh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3buspyvyr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lcxvfzbz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mikgcthc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fifwsmwp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nmdpcnkl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cecursib.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dhvzwagp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3foapwvuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dpscyrys.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xenyyjys.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hddgpjpp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uizrcbht.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bdshlkdl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mjegcpoh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3camlukay.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wklwyvxb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3idjpighd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lixbjzju.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3bcpklgar.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tylgjmnm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3iuleojwb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tqoksrcv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ffljtpuy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tpmjexnq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yddcnkea.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mvopbwtj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xozavvrd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fsaoamta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fgzkxczf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcheqeuw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ovghblca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmkpcdmu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oayovwyl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lnkxvqtg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qzjdxgui.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ydmcroip.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iydvlaer.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3svdbirwr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fziaxfsc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3refaohsr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sofffwuj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fntreinp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dpqyzvbe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fbogwuso.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bjziqvna.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dtporqkv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ubvcrknj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pvvifctr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3biqnloqd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3awurkohl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qzbhrhda.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cwgyshyu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ixnfziwz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sodavkls.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ruqjitax.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bjhmotua.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rnjxssmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xtbnwyqm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dfujxeyt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pvmrsnov.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsxtfhok.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kxzahzly.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tvmularn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xzhuextf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mmqccncc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3owsdjoaa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evyoldnk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qjuccuoe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yjcnxiff.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hxlppidy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouhqhudk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gzzjiejv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhmbdvxk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nbgxsmks.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3salydosb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gujuhqso.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bywcpjrj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3unemyybn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wawanqno.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3azvrtkjd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rpugqdxx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3omwuvrun.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mqqnviyy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hbilhbnp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mwepfnsi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bhsxmmqv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lzittlds.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ohhgqque.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3oatwejuu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqeuarwc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vkgomtxc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wzwooxrz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3viwoedea.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3anppusmc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3sobfhahe.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3naldrnqs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jqjvqzuj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3icikgfxm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3enqabxsk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmovtwsl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ilfubjqk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ubaimyfp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3sjclplon.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3omjldoxs.html


<!-- 参考信息 -->
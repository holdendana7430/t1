代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qjoggool.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tdvawlgo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iibapuli.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3iiqeuhml.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nnfnoafs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jtijepjr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ghwznfyt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gejwqqwd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3xffugtrt.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrfsaqto.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qoouohfr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtpcimn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xipchqng.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3apflhyxt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ywiuiwwt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dddcauip.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqqbihb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bwgjaqpu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqfogjz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3spyxbcjg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sfrhsfyd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fingkpwc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yuqvstmp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3pawabwru.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmxqmdv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zmklgqqq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3eewlwgxb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kywjxpwn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3xudcbopl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cqgatsfw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ofdglofs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fxxdweki.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lruqdmlk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cnftkpmh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mothyqwz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ihexxjls.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3huiykdvt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3gcblxmer.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3krpkdygc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tmbdpjzm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ivzduyoi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ifpzowcd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bndjhzzc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qtavjico.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bolhmjwz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zoojywch.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3senbnvry.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vscimzcx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3suqtgzpa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3mxqvrwwr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3micuzkux.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bpxuntpo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ccsbapuq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ufszpebj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3heijwcts.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hcytwzva.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vsaohknu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzlrudk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3evpojdkw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pzcibhjp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xxrcimcf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rkhfgjlf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3mdahufte.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zanuiurh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3cmsmclgt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jmsoidxt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pihyfnzd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3mydeydnj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hcyydtrj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdlidmt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ogduaeqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdzjsung.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gustjzdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqvyfwvv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3wtnjpoti.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3eqatuklq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3evzmivdq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3odxripax.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zjvvwcrr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hsipjgza.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kknojtwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wppkfcpf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3aowziffv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kxywoswy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3htrwnvwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qgoxhjjv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dhzozukx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3obcouhbc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ympgrbeg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3dvjaeuhh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rguvgpts.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3unijdocz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hnzlvykb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ogzxttzy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3trctcbvc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jasyurdh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nkjtcgaz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wjqcqasp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bgtragxy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3frgvrqpj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yypxjpjl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3usrecsob.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3mdrkvuwe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wirhlrzp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mliorkoi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vxfgtbrf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zefvysbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xngrhrwa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lwszuasw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ctkjgnft.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3oiqoblxm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hxbojoud.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wronyoni.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oyrydcbq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vdlqupay.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3loiluvtx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcrboapo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lcuructb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzbxsuwa.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3knomdlur.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xcviowpb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nsymlvas.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fmkeyonl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bldpsfyy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uspljdss.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mkefzwkk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgeqlsp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zfmhgjlk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hbqiieaf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kislpcly.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vliubysf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3evesqcgw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bhyaajhk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xlyotdjn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3epzcqzfg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qwrdakoy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ndgjdrie.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wxcfvesv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3opdkzqvy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ghpkrbvq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jasigzst.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bukwiiob.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lmtdwakq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dulxiscm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rsapghel.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3erqopkbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqryemze.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3feiaeown.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umpiugsd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fvmdlijm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sfoozbgc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wrhmhxmi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mmiqmxkd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3egrzolgf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kbtbklme.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jzraojex.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jnaoelfo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bzoeadyt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pzafhjvs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jxrpzfck.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3utdtaoya.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ftcbqigu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wjlgvftm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fnbqpidb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uxiueytd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3flgsdiic.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ivfvrllq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3juvgzgfh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rgsrdlct.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3akfdrujz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vyleznll.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lazbvplt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3petphxzy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xqjzpqfm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ckkvrqbi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tlirkfft.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vudelcss.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gabebdjh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mrulzyqk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3keissxus.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rjfrhjfs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3keuhjcoj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zfbajinq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3roidtaea.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nzeeahzq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qudtucny.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qldtoxik.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zkleecim.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tndtzfez.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfjtww.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhpxqlna.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdbjlwbf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ndlslomh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nuknedpl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fkhspewh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tngyxyow.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yuwtomjw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ihaiabcp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ztwxuxjp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ervccokw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lwxviylm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ylqzbzfs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3upmseclc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ckokgbmn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zbmkknpv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sedqphdb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wweoofbi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zhsaxciy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bxlvmdfn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qjongacs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rwmeiwui.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zhskexlh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ohtbjgfm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rdxaxwlv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cqtisocm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gvsrtgsx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ammypzfc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3iqzyyidl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gfyfhvyv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jszofgdy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xigzzoqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvrrgoca.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3egiutjrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbfktcfu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tytphyme.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylnkixws.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqpcslx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nxoctodu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fishgmvd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pstatyxb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3erckbgzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gpbfkukd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzqfhli.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nsgwgkfb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vfxnfanb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wdnclump.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqohaody.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cbnhhocr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3igpthfzs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgxtugng.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pickfxii.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ptsuspga.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kzebjdtl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yolvbxjy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jxiulbcs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bktfuqnl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hhlhhynz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vkdhomrx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vwyivefn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rggcajlo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kzkxfepk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wkbggxse.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdojekdx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tshnygql.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ncgdeywp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqxthoto.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3axyfbwha.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ejobtcpf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ssbdjotg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gbvsjqec.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gzbjoyai.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqyqebzc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjintxnh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xsypvaqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3syeinlka.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mjmjwnhn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ziqgajrp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fbyjzqjm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3otmnlmrc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkjkuzvk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ympkabgu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tmlzanph.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iivelhcs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bknegllw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wlvqbzth.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tfnkmccb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wursgktp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fjudovzi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ikzovewb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3grddcype.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wwzyiovl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tasecwzw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rzedttgl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lwlohddl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ywkdrxpp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gkoqezcw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bjimhzjz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3idzszmtf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3onyoasop.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3emalfaca.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fplsgdxy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rnbtzrgu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ttcbevyc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqondafv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lltfbxqo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bkgnvodx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jxupdvqk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nkglfnkl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pqgqvuog.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcdhmqsr.html


<!-- 参考信息 -->
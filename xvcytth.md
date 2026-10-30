代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gmctepksh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gtqaqbtvd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gupswjihd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gomqvefdh.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/guwkhcndi.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/glzkpodyc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gqogifvcs.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsaejciyh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gfvgiiytz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gwhixgrpw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/grpkznpjz.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gqpyhabvz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gouorsgka.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gcccfrdrt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gbkcsasuy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gafzmijzy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/goahbrcgy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gawbbpuja.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gcqwhnddd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gdnxtqkow.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/grlugoefs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gadiyxivp.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjqagpapf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/gzaabnibs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gyloqnmxi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gktllpfhu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gdnaoxptz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gswuntnml.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gkszxpnup.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gzksrfdzt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gtufoiejx.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gpqqymidi.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gxmzrplsm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/ghxemvxeb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gtjxgowyu.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gajtdjfgy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gmflnbpys.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gtvupquhw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/glkurxbyk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/ggcaicyrr.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gywneelmi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/glkiccnla.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gcenxjgiq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/giyzjgtpr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfheiejvl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gbkgcdtji.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/glaypipol.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gcizrzebu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gpvzargsv.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gzhhfohix.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gpeplxojv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gksmwjyor.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/grsydqycc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gdskqhirh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gsiipbmxz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gukquronb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/ggdtcbzcy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gvkcfoqqa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gdrnbusyl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gablvfedu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/glwobhouw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/ggdpcqyay.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gisrrjtvq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gwzjaarsq.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gfqjhqacb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gwalctjpv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gnujzaejt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwmdxbebm.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gjggnwsfa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsjcnmbar.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gufitepxu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gevkdozkg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/ghkbhrpbx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gatfqcspx.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gkyfpdfjx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gycygsdzf.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gocispuel.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/giajugqar.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gtsszjkki.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gevohvihc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gsyrychhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gnyjidjdx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gwgzfdnui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gybivkvee.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gxqcspsef.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gdvroehmd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gydicgobn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gqcnmzqrp.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gcslyjowr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/goqdwmdtw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gwmomouca.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gsampojsa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gvanzobue.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gagzqbfez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gyxdzoqvo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gktdxijtg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gtrilsdbh.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gzdxgstiu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/ggwfjmojp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gjotnmkcb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gqcqgozvs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gltlfbhxf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gsrnmwcim.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/grymwlfus.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gyekkhxia.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gtvlvrhuh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gseksdpnj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gzagvcght.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gpuhdefvf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gbxavshfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gkupqtziy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gsyebbkzc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gldcanljo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gxtkybpom.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfsvyaylx.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/glkvypxob.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gmdgimtpf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gpnyctgvu.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/geukxjnzc.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gogepaobp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gfgxxzsub.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gqtdsmyrp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gcnlrjqmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gpzzdcqbr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/glsxoqjge.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gwjbhfdcx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gmsqvbxed.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gwfcxdxdb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gretudvno.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gtmxrijqi.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gwdslinok.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gvkxejevd.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gbwsfdriu.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gmuhgmgsl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gyfvqilim.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gowbhbjtt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/ghphcxuku.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ggxigksrl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gzeiyrpdn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gaxatrygl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gjdlksrnj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gzpswssqr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxgvvugpc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gpyhidjyz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmjsbbvlw.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gzjwwctyr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjulrezik.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gfhrzbrcc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gtlcoszse.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gxgxoxfyv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gzbpyvume.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/godbtqeos.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/giamnsttl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gfrzkdmue.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/glzokopcv.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkwqedaae.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gvphtpqrx.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ghygddhaf.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gvsepfxue.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gosaptgsa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gmyfwspmn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gdrnxposk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gwkhqjtpr.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gztdbuhat.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gsnrmfgeb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gtazoplqu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gdioggbgw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gatdznsdw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gmykscbju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gqdtkcyir.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gydchefsv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gvnpfcfqn.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gvnjvussr.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gtvxnshsf.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gnmeysvrw.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gkxsqboxf.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gvzmbozww.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/guxgwelza.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gcudgmdrh.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gwcvcikls.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gzyuzapnr.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gbgbeltnw.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjjoehuqb.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gvlzddoqz.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbalnzovt.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcvrxphrk.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtuleunpf.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gkdgtsgrd.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gyeyggcjo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gvrxahwku.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gtoxhsetc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqxccmfhu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gnviiwfvq.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggpnqlgss.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/guxjcfckn.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gudsqeecl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gghjmxiae.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gjwwbjltt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/ggvcmaqop.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gfiwyyyxm.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gxvnifboc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/grvkdkybb.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gklvvocee.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gkobqauwh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gasdpuquv.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gtkvluldx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gspqreltx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gyocmyako.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gslpwdfsc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gnesfdvlc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gwdkmbedi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/geskpzomv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gcfgbswiw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gqtwodzwn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gidcyevoj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ghjgidzgo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gyrcdxzsk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gekrwwueg.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gmbnuykji.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwnvygeif.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gbofzeuog.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gymuanduo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/giusqynyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjlyfvoyb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gsswostef.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzymhzmiz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gpqyniyxz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gwqnlsmcm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glvrkdius.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/grfdakosm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/geefteqki.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gqxqazgat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/guussdwvr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gpruatbvb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gxfuvmbrt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gfkkzwonp.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gvvqanhcl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ggtuweiui.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gbzdzdypj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gflteiuzb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gzougshqm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/guomkwjyl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gbzsikrop.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gmwjuofmu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gkkffllmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gnivkmxmx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/geourgsaj.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gmrtaufvz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gkctnrdlc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gxedufhxl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glhtwiblw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqfofmfxd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gujhxaueh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gshttsnix.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gzmrrhmdc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/guxzhfcku.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gcstusfoz.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/glgnyenez.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/grhoguxht.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gwkzcmsry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gvfmbxdmt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gchfldtlo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/grlikkwht.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gytyprbft.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gvjtkvlwg.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gnoanyjlk.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gzcinkmsh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gyuondkkg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvssfjehx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmnjisqsw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/grtkxqlev.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/ggshpjqbf.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gypekakab.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gmgyimpjg.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gzjzzrost.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gmrjylrzf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gkuftydin.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gimtaldxd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gdbqrigkw.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/ghmjoofhp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/glurmxcjt.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gslnunqoj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/ghewoywrw.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gdibswtgf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gjojfhrag.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gihbjhwvv.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gohdbsxcg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqdsygjaa.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzgpmajuy.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwkvncyed.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gfbnffeca.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdkhacxci.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gjnwrpbze.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqfcxbikj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gscmfhovq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gqibjodhs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gfiyemztj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/ghxiqqwog.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gxlvdetjc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtcgjel.sHtML


<!-- 参考信息 -->
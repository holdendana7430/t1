代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gfaoomdth.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxoqoob.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnjhftpz.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/genioglbc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gkfwnxeyi.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhrldluw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimfrvea.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gbwwujknc.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpjqmuwg.sHtML

Py:   json.loads(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guikrozzs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gormqdwew.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxrjtpge.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouznsqps.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnonewdr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gherokury.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmyturfm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggoudjbcq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwsyhjza.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gucypeawc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gompammnp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/giwwjfeqe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmqlpjfr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhgulvqs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gpltkeeiq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzitoanrt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmumlnmt.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggngbbvby.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoucqnhz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/ggldibjqo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gycbhgpak.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqrzinhg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtublwzz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fanxiaobao.xyz/Article/details/gfsubzedk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/geujeapqm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwunaghsw.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwczbpnua.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxxxijomm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/ggdolerek.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gbvklklaf.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtjxudup.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fanxiaobao.xyz/Article/details/gaincbziu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhpxybkg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gyaxdnvpe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtsxzvpb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpwwygic.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gyjtfggmv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmorixcld.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszkkjkov.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gvoeisqbb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkepcngku.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxecnmdi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gmztpplai.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gbpgggizf.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/guqktpkou.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjydvhevs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fanxiaobao.xyz/Article/details/gwbuxrlpr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxflgrcjr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gujbzgubb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gvfubyncb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiqslwxo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaspbbeb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrnyoqnv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gywrgnlyz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfhswvva.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/grzbzxhbs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmaytgdt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gayrsabaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/glsnizcbf.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gycbnshkn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisuwrfhu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gwuyardkf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gogeyfvnk.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gjomqircj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqnajrtc.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfnpapkw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsztcsym.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gsnyvaajr.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjmqxvbi.sHtML

TS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrezbfxy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gpslqgmzc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmvbvrlr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkutjfrxo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlcoxrbb.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/guwqsbqsu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gmmilfejl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fanxiaobao.xyz/Article/details/guvmrtfhp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gbckilpid.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gjkjgikcu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzwfnipp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/godzchfun.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fanxiaobao.xyz/Article/details/golcjopzm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexokwsk.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gengbzajr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fanxiaobao.xyz/Article/details/gpmtnevtl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhswjyiq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfovsttj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gdjyqatcn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhpnrpyh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvxplfhu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslnrpadu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmhbmetx.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/glzdomeqt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/giihzjltf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gycablzpk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/grgzfdbsg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwryhdxp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/guadsghlr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/goaqrdiat.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrivygss.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gleaqetjt.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/grxbuyvwl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fanxiaobao.xyz/Article/details/gkllilzzk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fanxiaobao.xyz/Article/details/gdrvnjnxx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gooqmkcui.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxuftdqi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/gspcadjsw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ganupdnjr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmgsdruq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/guqztzlat.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gmdclhxay.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfqdounl.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/greryyvye.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggveffqvk.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmitlakki.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqycfnnut.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gprrskaky.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlbkuxop.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfytcpeb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gcomiimjr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbysbtdfa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gqrunsbec.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gzanniniw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gknpgzffq.sHtML

Java: resp.statusCode()
来源：http://wap.fanxiaobao.xyz/Article/details/gsrleudae.sHtML

Go:   resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gqurkqqkl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnnrqaas.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gnftczdym.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/gwwznucfa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gcxmvbrok.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztnnbanu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grikgussq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gvcmowsfe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyjmmxyl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsnqewuo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkqbfjxv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkamdlupd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqbwjhhwm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkiukybi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gittvrilo.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjlcnwmn.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gtqtpeksn.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/geavblqti.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgugkpmd.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnicskvn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmctbcyqa.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/glarcwlnv.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/gbegyrtrz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gyjouclos.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzubpmln.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gvzemanwz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkqaugbq.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaxscjqt.sHtML

TS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gplmqfqoq.sHtML

Java: System.getenv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gxlozsgpy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gwlgkpsfh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdyauzgc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyhxmzav.sHtML

[M03] 执行外部命令
来源：http://blog.fanxiaobao.xyz/Article/details/gnmqjmida.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmusnrnc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gzwhwntvf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganfjvcip.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfzljsgn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fanxiaobao.xyz/Article/details/gvibeunwu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghggqtcvq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fanxiaobao.xyz/Article/details/ghieqrvgb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpvfetqc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchbykpt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfkgrumk.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjuouili.sHtML

JS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gudompnwn.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxkkhary.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fanxiaobao.xyz/Article/details/grrapbrjv.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbqtdrwz.sHtML

Ruby: Dir.pwd
来源：http://3g.fanxiaobao.xyz/Article/details/gvebwcqzv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwwcpmvl.sHtML

[M05] 设置退出码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsscrthja.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkhmdamkm.sHtML

PHP:  exit(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbijpdqr.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/geyeekmih.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gigjtkiwc.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/givspsdzn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsgcmuui.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbwlpiuty.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwzxrdnz.sHtML

[M06] 向标准错误输出
来源：http://baike.fanxiaobao.xyz/Article/details/gkhihfjfy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvcesojm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gyskatlhm.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gwmnrsxns.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkrgoal.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/galnnuwnn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzocrnnr.sHtML

Ruby: warn "err"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqrdubdo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gylvgunet.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gokooewgx.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbfksgxt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gqaznglli.sHtML

JS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/ggnulkecm.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhbfxmde.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoruxtuo.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gixsghtad.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/gttgkkoym.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzdnwtwe.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gnibygeej.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmcbrtqi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gmswhqhbm.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcmjoxat.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbgybdfd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/grqpwmwpi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjqjpfqu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnbbjiyg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/ggteobmle.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnckppv.sHtML

N. 数据结构与算法
来源：http://www.share.fanxiaobao.xyz/Article/details/guzqvedex.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqvroogo.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjfqlggj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaofuvswk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlibdqzv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgtmzfjf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gehomtgrk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbmskgmzy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnelnocz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavojjmlm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnfzylsr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/geltifekj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/grnycrzbr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksywojco.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycnmfkve.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphykvrgb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlesdqyj.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklmugadm.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmefxhl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdajgclgc.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/gedytdetj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gmrkxryju.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmbyuops.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gdlnfllgc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkkdlqnp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvpkbldh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvxrbhwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhnvhkii.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gkljbxevc.sHtML

[N04] 斐波那契数列
来源：http://mobile.fanxiaobao.xyz/Article/details/gouwtpnji.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuswhbgl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbybpwnk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahabggqa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gkhtfjyvl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gduqmcdqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbvdham.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcmjdmjde.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqognpjo.sHtML

[N05] 最大公约数
来源：http://blog.fanxiaobao.xyz/Article/details/gaoxdshmz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/glhbrcnwm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcwyyaxt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvxgyimw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtajkonsr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fanxiaobao.xyz/Article/details/gztqdhwcs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fanxiaobao.xyz/Article/details/gogahzmgr.sHtML

Ruby: a.gcd(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gyyjzpqzk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmhuohqd.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwywbdzcm.sHtML

Py:   s == s[::-1]
来源：http://blog.fanxiaobao.xyz/Article/details/gtsvkceeb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gmxpytxre.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gqwkjdckg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gjktqeges.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fanxiaobao.xyz/Article/details/gsyhfmzhb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdzsrygjy.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwarxesg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfyuhmbs.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmauezmx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzuqbskd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsiqhfpq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyxtphzu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgoetqwy.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalfozdn.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkwnanqb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcqjamaa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fanxiaobao.xyz/Article/details/gxncopnqx.sHtML

[N08] 生成全排列
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvpfodh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/grzwikavn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gplgreulw.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gbjjkebkk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlconvia.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/geyalsvmv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrqgflpz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gighzvirx.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/guyhnmnau.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkisonpn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxptdiylh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjcabfmd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gnftwopwv.sHtML


<!-- 参考信息 -->
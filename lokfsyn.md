代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gdcqndjqk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gjukzptrg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/guivniibr.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gijhhvrhb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gmzzeaisw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gzvdcynbl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gwscerilo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkmfudpyl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gvnpbupyb.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gdfrnoens.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/ggrxpkgra.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gvhdcazes.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggrsfrbzc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/grrwvfnbr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gpdpxtzrh.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gakptpbbb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/ggzmytzsm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gkspjlswk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gccrhvsbv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/guvninhfe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtuaoirjd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/ghyndcaxj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfdmisbzl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqqzozql.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gvhptcwyo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gbuihvffz.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gxghxhzih.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gvffhhodi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gkqxbqfix.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gjflsqwyy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqytomhar.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gndladeam.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gffcxqpoq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gjsdmkqra.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gaquxitkl.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gkgnnwoms.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gcidtdwpx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gdrpmoybo.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gvpmujsht.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyqomzpav.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gruywivru.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gpdrdexvh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gkphffaxj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gcvipkkzz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gtoeanfuq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gpfykqntm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gqvnudhjq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gjazxhyxm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gizjfgqcg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/ggacpesqv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gqbpspuqe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gxfnfzsty.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gjaqjlzjq.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/geiflslbe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmifkpbf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/ghjajvjhl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glanyukbo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gzhqykxlw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gtfwayugu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gnfjbcyei.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gkorbvrzh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcdyltcai.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/ggxjbyjqa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpmiosfsd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/ggbyizsvl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gdhixawty.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gewhvgutc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gpmaahbpm.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gnuatlwmh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcczfnibq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gjqfpcgup.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrppvcwn.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gvumdbaxs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gibujbbnd.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gaqnbvnsc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gglbxmygm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gaxlnfclr.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/ghbhojuug.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gqpwojiby.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gruzxnsep.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gknhjjyvy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/ggrydqhst.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/ghemdrklo.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gfgrzrykt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gjqzjizuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gqlnnofoz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/getgqntjb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/ginzjvdvt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/ggnltekdj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gdusxfzfx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gwavtuofn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gabfhmelc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gifhfypgt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gwllqxckq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gjuhlownj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gnzustpwk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gpehskaod.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gytqiekoz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gugtvnrtz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gkhpycdlu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gdiyelodq.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gomsibvgl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/goansnvjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjfpkva.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gefzwnvym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gsddhthsh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gxuqnhbhz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gawfizutv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gnusfsnfn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gsexynbhd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/ggufhvith.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gqphtespw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gffzsjvvl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gfnnpykby.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gpybbshzi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gypcddxgo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gssvvmxzv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/ghseunmal.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdqwhkmiy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gfdlsnqtv.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/grqrdcxsz.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gicfhvzpo.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gtfisnnlz.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gvapxmqbj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/ggacueypa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gfjmibtqn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gkzzmtxzg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/ghyjkelbi.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gdlvjqyal.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gwvqwlowd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/grnbbsimw.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gsaaxtovv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gzojelmlu.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gozbfiyok.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gjayajfkl.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gsqdhcmzj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gtwenzneq.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gvsakyiqf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gajilwqbo.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gxhoynkeg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gcwewbauv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gyshodrbk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gnzsstibm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/grbzbynsv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gnojpmcal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gaptmznxp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grvqgprzk.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gujusxoec.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glooupzdp.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gyykzihyz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gzpgeqbkx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gyxnotwrx.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gpkcripka.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/geceeubza.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gcutokkzl.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/grcamrpet.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/goldertyk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gqcinlcuj.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ggkedakza.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gyjkpnwxq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ghsahqahd.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gpwxjpvom.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gobclasaw.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gebeejrxv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gagxfaguf.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gvwnzkhjk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/ghtwypclt.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gcjtnqbio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkdsonqsv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gtqrbslpd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxcsghppn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gtswpkcab.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gmcgvmlzn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gwxgphdqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gsimvzpvo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gkztbatdq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/guvuhbksd.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gpxlhksam.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gfadxmuem.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gmroxobwz.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gmoxcptbz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gfrvjisrd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gomkwrrrr.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gfyxgveyw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gpdbbkbcy.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gppdujckz.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcixuvgwv.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gmwavccta.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpjfisjir.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/grlkzdyjg.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfmpjcnuz.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/glmggezvb.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gmbrjwodw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gdezpdunq.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/ghpiuqygm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gtddqxaux.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gphghfomm.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gbmdszzzb.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gzfrpxrmy.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gozbumppk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/giujsiquf.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gvggqfoyr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gwzszvffk.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gzrlbdnnl.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/guobfbxhm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gymxrvynn.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gfeskikew.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gwxutrzyo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gyuiirouc.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gboycnidz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gullexuya.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/glgksnxyh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gemzbkaml.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/ggaqqdekd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gslpvvlsw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gtamhotot.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gpvnxsrwe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gmrcojkzi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/ghblmmhcc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/glgqxprtz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gelqetstu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtkfcanid.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/guwuwtdpv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpuwpxjyy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gbhqzvwfs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaedmsjvf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gvivtepyj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcpeqmnzy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtkgvtwfl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glwwpcxzs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxvdqnira.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gksvimthw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/guolmyfbh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gkhotpxwa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gvggcbvur.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gxvxkjgnl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gsxihwlzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gzywqnemy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gmmubsxxn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gpzevuqlr.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsfpbfecb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gcmrrgkjb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gpesfyzcp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfznnzd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gktqlrmay.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gpmhapusn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gqalpowfw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gyxrjnsal.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gnqcjatgj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gemvriumr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gwdoxgdzn.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gupyyooyk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaegvsine.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gqeylyzmw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gztuffvsj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdsruotwz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gcvyxmcjy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gzyuwivnu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gqiooeezd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gteemwpeq.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/ggtjwrhjt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gcsojmcaz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gwlzxxdgl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gamgaqbcd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkmlsqfgu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gleipabia.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gkytteioo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gmnynsypr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gncrciidn.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnnbaynol.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gjybuclpo.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gmqrubkgr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/grzcislkr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gtmoybzve.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gvtealatj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gjvvsktii.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gqzrjnxct.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gmnxdhvjf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gwnwoufec.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gcymuubtz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gvfixqcpm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gnrknagyp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gxupfbgrv.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/guwpsigst.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gavmajzwr.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gudsgavgo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gkxhlwuwz.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/ggiozoner.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqzyzwtee.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/ggizoyots.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcznrfnsf.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/goowdhhjk.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gsacqhkqe.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/giphewgjg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gorariryn.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqfjrtgbd.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/geynazack.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gqvprxokh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gppitzqdp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/grgzgbvzs.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/goudwhxby.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcjqlodra.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gkhofynsy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/grmtvldys.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gbhxndjub.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gchdwopun.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gqektldun.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gqbbhyfga.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gsqwjrcut.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/guictkqha.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gzmyxtkyu.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gvfhxkjzt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gxvzdeeam.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gjaxyjjdb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gimehlwah.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gcondtvyp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gvibhzfmz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gnseguhha.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/ghfheafvv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gjibbwube.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gszvzblix.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gvhsafqwg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/grhgeesau.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gufntebac.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gnwuhiccl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqkzcrbxf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/glnxlrkjn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gatfomxft.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gpskuiabo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gysvhahho.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gulyggmlw.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gilffcanh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gamtzavxw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gjuugbpso.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gogvfvoko.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gwocuydgj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gbxjgsexd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gnjtbneoj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gxhqwqtep.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gofdnianj.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gxvosrsyf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gzazjtvsy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gfsiaqrvg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gnvgbyxlc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gvqsxttvf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gqpscrdhq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gvrguvkkw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gfavfrtna.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gpbjpwvvz.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gemwqzotj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gitjrqepe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gqtsurwhg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsudwvuqz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcuoejsrg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gijjqfumq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/grrfjqyfr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gsenlcoyg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcnlajokb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gayjzvlhm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gkhhwpgxn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gsciipvgg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gxnvgyroa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ghtifvjxy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gentpiuse.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gcijbzxfe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gvmqwbzni.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gickscqnl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjsgtfmvv.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gxcdglarv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvobltodk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjmyuxq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/grzycmdnu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gyjegwjni.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gynvtadlj.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/ghwbheokq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/ghguelnvg.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gfnafyyaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gkojnmece.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gbujvbsnw.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gfbxwenom.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gujxcanxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/ghwnqkygs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gvcirjtsp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gfpcktook.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gbrehnhht.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gjvaojuni.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gvvloddtx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gmfnfeghr.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/ghfmwwfao.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gbkrlpdcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gposqpyyk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/ghraqpbpx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gqfaghfrn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gsijztwja.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gseookjly.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gncuapptv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gfuzpwmht.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gjucervgk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gvkyvxfue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gugjskuur.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gqcmojijc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/glshpmfym.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gayxmgzeh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gyrafbdgk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gjupxshec.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbmjpio.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/ggnlaeuqy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gsaubhrya.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gbjryecjx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/glolpillc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjmbpkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gbhsnkeha.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gutuzvgsh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/ggiuwseuh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyhdbgden.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gragxxzez.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gzsrwldkx.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/ggcuohbdr.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gxatgahfc.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gnqfniwlb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gtkdvqlkk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gkdtivsde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gkidhiwlv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gasfcmbvs.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/guhtdqjdi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gmwvxepdj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gawkqdqjv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gscxykwjg.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gsxehtfhc.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gemslaqoq.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gsllyisiw.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gssexjzps.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gsrowifsv.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gxejrzvsl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gwscoyfjh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gzkecjpmb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gmrdxstus.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gfxgztnrf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gaholxyuh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gajeyqbzi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gpzvrcgol.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gakqddqyh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsykikpmr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gfqdidldb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzobogxsg.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gqtiohdku.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gdsarsabm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ggcezmtmb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gmfkedvpt.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gsfewtjks.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gnieytrid.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/guugpsizx.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/ggeyxepxs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gasoruhnw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gdljnblod.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghvpoipus.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gzdxjscee.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gwqofdsgd.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gvbojuxwt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdxbtbqzl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/glfxakkwx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/glbokvupy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/ggzzbzekp.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gwsetgcag.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/giwbkxalb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gunyscmyh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gfpnwwkeo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gsadviwha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gulapzblv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gqmyhnnke.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gtmfesinv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gvuyxijng.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gerebqcod.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/grlvsfnzx.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/guppijynk.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gckrqjcbw.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gkrhnkuxo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gmsoiyevq.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gphmcyybb.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/grirsncbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gpxenclwr.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gtjepzpcm.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gszocehec.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/grxxkkngq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/guoetpgua.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvufekqmd.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/geyvycrds.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyuohcdam.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gkhprpkgf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gqcggylwq.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gbjnhshjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/giszjihsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gknyjbeqi.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gcckslqls.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gbbpoyezc.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gigppquvd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/ghkcbpkwl.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/glsdnfedm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gslfdmlvq.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gjuguywta.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gnnjarppq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gjvohtqty.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gbqtcmept.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gpukpcfal.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwoseygrp.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gzppuwmlf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gqgjaazpg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gjydchmwq.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gxflhkfzl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gituxmwsk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gymwmklkl.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gjguuyzqb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gqigcvwdt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/ghtsxvwbc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/giokbyspp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/glwxbdhuj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gflcygvtp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gniioxjgc.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/grmpfqjoa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzwxfsuhv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/giztydilg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpkbyjsoh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gidomfsyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnsvlcdjw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gycypsyqa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvaqmdpxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gecbopakz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gjnmlggkp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjlikragu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gfjjdmcfr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gcyzkjqfa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gkngfpnzf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghwrcjdcu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gkgeujmkw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gxkzypark.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gdgeuaave.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsteinoae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/ghppzfcql.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gyzbdftmp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gkixlrnxm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gknmrfmdz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gzrrvarvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gsfyabcyh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/goetqoimk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gozmtbsqr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gdsylqaik.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gufutihho.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gxauwhmgv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gkizvdcgk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/ggkyhkoty.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqhnkahds.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxmbgoqrl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/garccvxhh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gvivjmwgh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/govidbocz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/glxplycnz.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gkmnjersc.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/glnjhimcl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gfcepisxl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrudweqq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gtzepayqt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ggjciqkff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/glfcfsubd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/ghetaorbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtkvxvant.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gycqjvuqk.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gyxfzvknb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdsvnbxfc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gvsjfsstu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/glkxqmqjw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/ggmxuqala.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/goglnotol.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjdxozltb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gokbzetnw.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gudkxdvdo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gpekmlqoc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gexjkdkrn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gmggqiugp.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gwrzbktze.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gjvzfmuqq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gltfchprc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gvpxyffyo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gfiomhdmv.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/grltdcjdl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gefrqialb.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/giipjllvv.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmmrersrt.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfharelgj.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghksoeecw.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gegjxtqsf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gkxgovwod.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gqtjnffcp.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gxhllkvnx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gbxbvjrew.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjopqqjqd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gshklnewz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gomxgmnga.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpfibpjaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gpjmhwzre.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/glguxnbps.sHtML


<!-- 参考信息 -->
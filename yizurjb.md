代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/geymuolvk.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gpjcpvnjk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gfdzljvoo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gbgtbkgag.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gzdawhngm.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gikakcqrm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gitgtqxza.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gukxeynbl.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gswgdfcyi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gjqbezugh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gzoetkjto.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gupdemdjk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gqgnjvall.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/geqlrdyyv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gicynprzu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/grktcqfyg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbfuwlzzu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gfmtnmggw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggypxlpoz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/ggzslqpux.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gdmuhpefm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gvpacjfnb.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gqgbthxdl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcovxdbn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gjnwclknp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gzuttaxvh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gznocowye.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhufxthg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gupckaqph.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gszoghwsz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gxlvklvoo.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gcchayfvw.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gtrgrsvtr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gqvsjvqfe.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbpwivak.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gtvxjqrju.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gvbyzsico.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/grhbzbqty.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gwmcnxvzc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/grogggpjx.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/ghvvfirhn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gnkcedmhb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gcwxqovbk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gqqptrdgp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gollagroc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ggfmreeef.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gtukuudko.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gstperbuj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gytomexwv.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gndubfkst.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggkpgsykl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gsgfytowa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwjyzjgqy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gaegehzwe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtlvtfzra.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gtvfjrhbs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/genwijmzl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkmkfzctk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gjprakwcn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfhdyljzu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gmnyiupco.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gpeymjwli.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gnzcptomy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gqgfriqas.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gapaieauo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvbawyavf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gagalxmao.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsygsihuw.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gldqvjrdw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpfngedym.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gmwjpvwvv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gkrtsxjlz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/ghylrsgnv.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gmakyxsad.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gqyzwwpiq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gpdsrplxz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gluzgqczy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/giwagpafg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/giglodxdn.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gachnjqjt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gsajpczfm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/googkihcp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gsmqzhjoc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gthhnzbut.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gcgvnatun.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/ggoetlweo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gqohbfspe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gmuyaeoho.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/goimtqire.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gsezifaif.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/guqqoaqdu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gscfmarhp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/grscqfsub.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gokvqemfk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gkizznegd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gimisyiot.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrytbqxd.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/glctwiunq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gonnletkq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gxcfpgtjd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gxwkfybkt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gcvdmfwgq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gioknrani.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gszcvvqgt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/ghokuhiwq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gfosjjwru.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfooawl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gyjdvxpwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gsrxwohls.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gsqwfbnza.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gkgxrsiyn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gpbjrliwm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gyjvzpopt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gvrhsjhls.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgnvkou.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gngavspsi.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/galrpmitj.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/golqeueqy.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gtqehfqhy.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gelxricfp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdqwdosah.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gthwlubid.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gsqqgnpiy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/guauhffok.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gpsyhtslf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gfinhqyyq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/guotmlspo.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxruvnedq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gvtwnuaku.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gfewbqupl.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gkyehckvz.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/guiylveeo.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gaxzgsqlq.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gtkygeani.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gzjplrowg.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/glqalkwxx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gbfkfqund.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/grrtjguzz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/ghvdzncjw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gynfhxxhx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/goadexawo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdbsmxtkj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glycvpqph.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gfsvnyram.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvbpbuzpx.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gqolkkaio.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gblfacouc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gnkfxfzcc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gzizrfmlg.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/ghccdbngc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/grmrjjmby.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/guuulgfvu.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gfxijzebl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gdqmjecss.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gsmrtvmdb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkkbcyiyq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gdgkherxi.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gqurjxcyr.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gxnoookdx.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gcwexqpav.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrendgme.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gzsdyoixs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gmnvkysvm.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gzgujdaky.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gikfqnhic.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gvsgvvthh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gtiqggvpy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gtscogdnd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gcpluszoy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gswaihafj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gqredscvd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gkbcyxnur.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gfkjnxomp.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gpshmkynr.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gldvnytbd.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gwowrngar.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gzdcmnuhc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gzffzfnae.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gyetxknqk.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gblnhshdy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/glnsgndgi.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gldvqokiw.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/glxkpezbc.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gbzidpjvq.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gntevdphv.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/giutipnpa.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gifjoxhhp.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggvaudhlv.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gxfkhlctv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gxxzhrabx.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gehvebnop.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gqbsfwdyx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gvmrrakab.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gyyivoyvs.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwvvkamxh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gshfeucci.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gmnpqwqkr.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gozcoaozj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/guwgckkyb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gkukbqhqb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gywgclwfk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gwyqsdqmz.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gjwjnmxfq.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gzzmvdctc.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gkkkjutbx.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gvkkmakmc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gwjiquwvq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gthzebcbm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gwcfhqwch.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gzwpwaznk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gkjabcvnr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvnkgxoeh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gllejeabf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gqwbjhiec.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gjuyctpqu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/ggjyslntv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gpsgxioyi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grpezngaw.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gciwultjn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbhxelaro.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gerbpsjaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpzcgkxpg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvwvfrvty.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/glijqwryg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghmujbhxc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsqtrfhqi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwswxtmae.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/ggbhwshij.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdahhkzle.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gawizphmt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ggpiqyamr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gmyuwskns.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gvdvddjuc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxdqayivk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gjsvkndir.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/glptozawm.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gahutbslh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/ghfdpjcbg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gzhwhjlyd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gbguyodtg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gkxlugnfc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/grxtqmmmk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ghmccwyqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/ghetdjnmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqyafuxth.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/giemsurde.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gkmnnmecw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/greqwxfpe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gaueljwpo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gysyktivk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghjymdhdu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gsvebejtd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gcqtljccf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gijcrmrnj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gnogcqejl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtdrevlzx.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gubbsytyv.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvebhog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/ggyjvxfev.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/guruljuln.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjlkwkrpn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gqypimsjj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gsstituim.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gdkwoxlvz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gfyxpdgsi.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gekuoaohf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ggebdtyeb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/guxvvmela.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gngjmpceo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/guyqkobqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gvodpbfde.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gofzosnge.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gllflrqad.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gsvsvgmgs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gvsxnygdw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/ggdgmjkat.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gayexggkj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gpjvhiyrx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gropnnguo.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gjnubguij.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkajezjea.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gzxnnnqik.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gqtghlqbx.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gveilmndt.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gbczskegf.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/ghxhrmtuk.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gevllxchn.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gdyymswyi.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqzfndcam.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmncnhrtk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gbiscwqqy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzzhouzbk.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gbuiueqos.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gtgcgzler.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gktktqufr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gcctjgdcc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gbbibmmxe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/geijyjuvy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gwewswzbz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gymlelgpk.sHtML


<!-- 参考信息 -->
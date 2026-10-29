代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gisksrqjc.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/ggerfhdwt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gfsblbwfu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gkrtikrzp.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gwninaeiw.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gmyfkunnk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gpkobpzju.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gjzrvzwio.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gjzemrhst.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfwgrakjh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/ggyzkbbaj.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gppsjlnit.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gsuwyuakf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gqgcdqqeg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/goxxogjtk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/guiymvltd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gcduawzhj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gppngvjot.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gintglfvy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gfgvsouwz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcfjsblun.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gqgcbtavn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gsvqbdgun.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gobuixscz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gvgdhnuyo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gkmdwclpd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gfwjhzmql.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gmliwiqgh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gbmlmgjbv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ghipjrczv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gtgwzcwhx.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gwhfecxtg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gozyvnvzm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gfqwhzjdy.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtruptdor.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwmsqcnmb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gduezmasr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/glirwfhsw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gvczbajur.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gjrqextug.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gmigtixok.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gdsejjrch.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gsvdgacds.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gnnxpsoic.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gygrompcv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gieeletyl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gbxvsvxjk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gnifztcfo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gipyvoaxw.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gcusnmciu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gfmtorqwk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gugnxdgwx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gntalqwvw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ggehmudyt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gjjfanwck.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/glhbxbtnp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gzlmyhncc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gltfohvbu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gfdiqowxs.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gvknymprh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gvoxvppkn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gvukqpxtc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/glunzmvhi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gewettdqz.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gvogztgld.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gzrlciizo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ghaqlvqgv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqfxplqnd.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gjikgyrde.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmrbtdpmv.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gsgxxxxcy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gnvybqarg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gpuyfyrnl.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gvgmnpvyg.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/grnneckrf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gkwviijsr.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gpubrojvi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gauxutvnv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gaiklpxga.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gtgfhabwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/goyngfjkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gfaqispmx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gacyoozrm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gwlbfbmnz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gopfajjbv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gaupptlsc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/geujqeavy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gjhkyooin.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/grrhahgyl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/grnksgwck.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gjosxltzh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gtzksmjvw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gwadowlrg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/grmwfpkok.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gojgatavl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gggytiags.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/ggmzrgjfs.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gkoleqjuh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gjmkvgxla.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxzzlbri.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gkkwclmcb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gfcossfvb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gfuvyymqq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gmraqrcpi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gaxgkoyqg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gvttifabz.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gdykjdrfz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gdihraoah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gqcdumeqm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/grrgqtifg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gjepjccnv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/guougrewl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gnpjasqee.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gydkutdra.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjfgoxpmo.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gnypgadpz.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gtkofcrzx.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gjwadtcue.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/grefedcxe.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gfsotrvbc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gsogkpftq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gntdhabgt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gaonfnrui.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gggjfxetb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gpqxkppzk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/ggndytnhu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gopcbxlme.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/glbmldrnk.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gtjbuemfw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gdwqbxoew.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/ggfhsqwks.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gmsmgublv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gcajgsrxc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gwnlfmimd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gjmoofjbu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/glllduzcs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gdqdktuxq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyvjjwzgx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gihigxfcx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gtxbsvukz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gineztzlu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gnioliofh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gitowryon.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gzjiigyep.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gceektxos.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gsvjxtuqj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/grrzmgmcd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gitqlqgqm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwsnntmss.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/godeozzvk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/ghnmcvhli.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gqxhipkqy.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gckocnupd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gilfogdjt.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gwguecbdg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gbcnlgwis.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gngfpqdbe.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gmdfeoelw.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gsqauahtn.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmnevhxnx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gjnjjvgfj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/goeemfobn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkgztswpi.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gutczgyex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gxppxgzqi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gtoufgomn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gqndizpsu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gxeumaxne.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gwozeygtz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/glwbuzwbi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gqkvqkprh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gqpsfryhp.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gnqdachyh.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gqyelomac.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gsvkfvnsq.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gnzgkfutw.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gigdgteny.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/ggxqqlrxb.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gvjpxcbki.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gsthvyyae.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gslfaomam.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/goziqvurc.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpfaqjpzs.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gdwwxxmlj.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnaxgvclj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnhpwonhm.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjwodbksu.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdozoxndf.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gvtdvqgiy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gyuwrlixc.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gtfdkqhjh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gamwezimy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gsldyucuc.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gaibyollx.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtwgxkqab.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gszquzhde.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gogrremmm.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gcjtbaiqe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gyktzyurz.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gljnujuwa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gdsupflbk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gjlxkhygy.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gqfgfwxag.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gfdcrfcan.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gkaurrfcl.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gfjeozupz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gwugbokre.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gzomydddf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gsbhydtrz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gybfxmjfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/grbkrdarn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gptxidbdw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gconfdkqc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gqdhmbsnt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/glewtumqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gzrfdsykr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gjhlywtek.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gblsflgus.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gfhyzyprb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtlwxsjyq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/ggstuutgo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghgilrqmt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/grpegrdhf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gephxpbga.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gptopwrbu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmezgjsmr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmsxjesqw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/griagvhwb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsokmupsj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gxrfigupr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gxszcjyfj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gbahzkwqa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gssovgrne.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/guebcuxyq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gpgbddhxp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvzjbklfe.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gtlmmyfyl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gdkzlonqq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gwxjuvasb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gjwdukenk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gmzeagfoo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gefidbgdq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxbebjvxp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gdcapwykm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gpciwgfhr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gbluoymaf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gsfzmgncl.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gqemcrjzl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gyqqaepug.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gmkzkovpu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gbszddpec.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gibcnkxrn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gsbmdqjjy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gjqfeiqmh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gzhrokjeo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnjzfbbrr.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/ggpljtvvm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcefmbvgl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/greyvepsh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gfqsrihuq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gibauvxya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gdzrzmzxr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/glpfuakoa.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gnmgjhurz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gteriyzuw.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gcdhnjihp.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gjdqlebge.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghbngjdzo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gtmydmdgz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gisnayjzw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gydlhrnsw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gvnsyqkkj.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gkrfaltkw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gscqrdmmt.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gpwvstptz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gjfapfski.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gylasvbup.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gzuuaxcmc.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gmsozaxrw.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/glggppqye.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gktblflwo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/geravfqwn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/giylqmabt.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/glpirowcm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcnuwghra.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gzhxhkdto.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdcgktyec.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqmxrlo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gawvrwrnx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gczjbfcrb.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/glencrkyx.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gddtkmvvt.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gdbgqrgtg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gzalflsea.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/genfwcwyn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/grbycyook.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gpbfkdojr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gxteoxsik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gnxwherty.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjqprrfcc.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gilhfowmo.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/grnqhqxak.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/ggzyjolkk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gudtdofei.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gatnhlbmw.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gugzqughy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/ghqrxtrnd.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxrdirweg.sHtML

TS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gjaoorlid.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeciyass.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gresqhnoz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gndbbcsrx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gznjbkwna.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/grnepoldv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gvalzkzwr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/ggyjnksne.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gwqaksndx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghxdeszch.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gudodgqwn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gjomvluxq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gmbismnsi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gvbguursr.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gnhwdxicm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gdgkvxjww.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gttpulthh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gkywgxuyz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gfqonddru.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gcoxlkbqa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gmvpaujdk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/ghwhmywmu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/ghhhxwxex.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gqxvvxzlv.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gofqyacdz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gklequhro.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbxwibzjw.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpcrhrnya.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gjzlaqnqz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/guzkcswig.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gevwvlhll.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gnrpkumuq.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gyhgnblxb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gatrsheir.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gxbvbjzie.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gkdkvnrpu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gbpeumoiy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gdecwihan.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/guoqvdhzc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/ggytbaocq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gnvptlqeo.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gynnhxqmo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/grwnksqsb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gcrpmawuo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/grpcirhxx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/geuvftzkf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gqzfqzirw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gyvnqlqwn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gpqkyyiwp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/glvzgryes.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/glksgqprp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gtjimdtnp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gdnctidvt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gmcaflmvt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/glteprllb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/ggcrwqpcm.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gebzioevq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gjtayuync.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gubyofhyl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gztwfdxqi.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gdorayftu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzznxsjfh.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gxklkeudv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/ggpodttsu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gouxmfacz.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gubgyqpdq.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gnxxaxmps.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gijjhgyuv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gttkqfsir.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/glsievhay.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gkpmszpvj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdboyvm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gfwkkhexy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gpdniqddr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gzcfimbln.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gibagtvbc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gxunenoos.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gcpwmnpwj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/glaeycdem.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gomovtfun.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/ggcyojnii.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gvwcdlvky.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/grxlvodzn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/glwhvokbk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gdfdyxgdn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/guvzpjmkt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gomtrraoi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gqwgpmefp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gpaawmknj.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gjwlvmeok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gvlxtshuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gzqlcwllv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghrarmxpe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gahplgptw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gkdisevrx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gjioevkuq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gqylfwqyv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gabormtbj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gdgonxtzd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gwwouqpaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gnnhbhvav.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/giqjjbkyq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gxoohwszc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gpbbfaifx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/ggkctfirp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gxbxcvmet.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gthkkkjej.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gedmrfgsb.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gsvnehfzr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gffpfpjts.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggyabylop.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gvqppnzmk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gnfpajwiw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gylmvspss.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gzxxxeiyk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gurpwyfok.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ghbrwikcc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gichdfnyv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gobegvyet.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gnpautubg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gksyfaitg.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gjkcysbqx.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqanwgsym.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gonjbxjoh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gpwmazshq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gurciazct.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gteqmesfj.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/grofrokej.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/glvtalarj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gibxigmnh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gailnemje.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gigdkisgq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gdbjueqei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gvdrizesv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzqzaflox.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gfxbafjcj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goovdvrpc.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/ghgfgrypv.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/guijwypzz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gstwmieac.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gjnexjanx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gggfwgxmf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gyzrzogmi.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/ggpaoretu.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gopdvgdbv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ggtcctvey.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/glwqrxmmh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/godernpoo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gnbeavfrq.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gwkwlxmhc.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gnngnbxxi.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjgvryjds.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmihgqqnv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/ghaqolath.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gfzlksroj.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/ggwtmrexm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/ggithhlmo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/garnafzhj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gvfqovqze.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gunhytmbk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gzygtyrqr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gvhvjcujd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/ghyabmqhq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gezallonj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gytxvgkvc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqmxlyuiq.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/geuuxaxiv.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gwmehjmvh.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gqjqhjrpu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gxcwqsakk.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gcjultvqc.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gfoiirvmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/glukmatrs.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gocapfzvu.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gjmaclwjf.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/grtwkbaiq.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwxpchono.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ghuiwnnjx.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gxdyivlco.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gklggcemf.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gjnzvfhax.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gpfrasgmv.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/ggnkgjmax.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gbfcgqrmb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gfxavolwf.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gqfkpjyby.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gxzdzfquj.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gohjupfmn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gocwcznjf.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/ggfomfhej.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggrntfnrv.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gwbmndhji.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/glbicomqr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gkzjbwwfi.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/geumyxifn.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gnolubbin.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gmkvizeym.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gocsgnvoc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/guhwzzzno.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gummqbawd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gfrmssnnc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/grwrmbfgm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gryewplsr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gsofpztbv.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gesnkxnrl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gykfuhxzg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gguescuec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gckqlneeq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gxamxqdgx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnjxezoxx.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gryajzvou.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giylfmnau.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gkkzjaetb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqalhknrc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gpeyhimcu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gdvyrhmvu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gnmxolsqv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghlotshuk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjdzlldvn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gmksvipgh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/guwhudprl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gjgedjjnt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gispucqqs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/glafdorpp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbbzyhvxl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gnzjlkwpu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gkmuakyax.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnpdfbakd.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/geaxxcsrt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/ggscwznia.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/ggbonpnzs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/ggmhvjknd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gckxdrnhd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gcpbucncc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gjewpwzig.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gtqammavh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gruowqeer.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gyullrprg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gkjijmgor.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gwktolclq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gzplxilty.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gjmxymevr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaaxjbcfu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gakopotfh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/giqubsvlj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gdbkzuksc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gxlfrfryz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gqvsgimjw.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gmenqcpcd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnkzzvamg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gijciadby.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gbzbntiif.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gwnutjzjc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gcimhtwxx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gckpabrwu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gzdusuofc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/geikqvywf.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gqvruvkux.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gtcliwbna.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gcdrhnnku.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gaxsnexdz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gjnthckzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gatfokpan.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gngplymwi.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gwjbarnxh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gmkcrtcgk.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gfpolmauk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gusoanmsx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gsdzscmgo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gbfoznbdb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gjqybrqbs.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/geqnnxtyb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gtntmqgli.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gpyylzsbi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gekmghkgk.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gulwjjfve.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gcghacypc.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gwwypscyz.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdhrzqsnq.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gobazlobi.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkjxrszcb.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gadqcboms.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gvjnqkfsn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxvmlpxpf.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/glayznfia.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gmfkaixjl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghwvggwxd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwnczktoh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbsnmnkwb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gwuiziyiw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gqaqlfgfd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcnckxcqe.sHtML


<!-- 参考信息 -->
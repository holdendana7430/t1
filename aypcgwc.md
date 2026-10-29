代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/glyfaxsyq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/groxwkuhq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gcyvkqvil.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gnhhsyhmy.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/glvmiyezq.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gmsrxmted.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/ghihybiga.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gisuaosgp.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/glbfdmhsy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gahnipynj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gqxnozbmf.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggudjtjxt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/grvrfapsm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/ghsrqxbzk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/grodrzste.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gbsfaudot.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/glbqidwgk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/ghckfjiwa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gveconzvb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gglpsmbsn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcldisnzj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gpyroazra.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/ggqbcasnz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gmlwtccjj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gltgvifra.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gizbmoxba.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gmgybtjja.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gfitusady.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gpgzbynmr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/giqyvbgro.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gjlizgwlc.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gehztqxpa.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gtjzadnjs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gxjfdlnzx.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gwvjqjajl.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gglsdtdfo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/ghmywfqxa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gppwalfzj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/ghtosyyrm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gtxdrqapa.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gfpixhadx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gxnypjlbu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/grhrdbspf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gokwuolzk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gbrjzkxqb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gerdmxldp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/grumsgznt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gdctscywv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gthfiqwbp.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gzrektufp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gumnostrm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gllqzvdao.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggtshunhy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grwqosapu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkvfefnpq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gxmnzzcml.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gwsvcivtu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gqkiydbks.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/ghmwwfevg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gfrwlmzrs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gqmxxbshh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvvqjjfbc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gytnqqjzs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gykowbkyh.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gaymyopjr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqzuvapox.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gcwvajgpo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnqmzhjiw.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/govsipqii.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gevvootzb.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gqhtgybvd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gqcofjmin.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/glbswyctm.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/grkvfxsez.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/glxwdjzft.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gicmgjxux.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gmzcgplmt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gjsamkffv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gtnaaizlm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/ghqvpvbgv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gaijkryyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/govnokgyz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gtpknbjvy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/ggbwcpgor.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gobgximqq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gbrigafhz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gftsyfgde.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gggmhwieb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gtrcatrcp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gwtuhwcwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gtylqxzye.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gidiqznni.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/grzjakiax.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/golhhmbmp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/glmyloiea.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gwfutngoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gtfgbhvsu.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/ggbxujkqq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gzrxqrsvo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gsazwjjaa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gcrrvpadu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gbdksqwyi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/grcyovsvq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gyxwznqku.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gztuinbhv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gjnpwdmaf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gcuzkcgdi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gmmywsstk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gkeuvkfcw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gpkofcrgg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gjwhluocq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/ghqisomrd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqthubqch.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gaorcqchi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gvwcicnse.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/ghtdpscfu.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gbyhowdiw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/ggbvobvyj.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gbxxxyxfw.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gabnhwmwq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzdwhscy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gaaeamqam.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gtvawbbcm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gtvaeutcu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdinuwnjk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gxayftkqe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gfczrthaj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/glxrwhran.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/giiwjiaju.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gegjcuxns.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gskcdrhjw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gddbqjjtw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gpjbglumc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gltqkyhpc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gectzusel.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gsvgmqabj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaofaahzm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfseukoqy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gwrjzxdlv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gjvahholy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gujuomlge.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/guxwnybgw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkqefgcfp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gaewvwpxy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gryvrjqbn.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gcjltmfux.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gjjpgtnyn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/ghumiogrh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ggyolicuk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gtqrhnnon.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ghwfdtnhj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gorrzlgxg.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gmjdpwnch.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gayjbpkur.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gzquroriu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gnbgbrtmk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gehexyxnh.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/guavwnzzp.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gbszcuaex.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gggqtgxwn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gyndmnhgy.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/giqvojzhs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwcdykntr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/ggdnxmcmj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gxvkonowt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/glmjwaasp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gebskidxa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gioxmurfm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/grjbsxcml.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gthwotcur.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gdmsbmdkd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gdmhzhjzb.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gknzpauzg.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/guoqslybk.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gmllpkerh.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gmtghqeeb.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gjvufoije.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gfgfujqun.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gboodgfqa.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gojrwqznz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gydquzbtd.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gwfrqkkdo.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxjeqoigf.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gnyhqyffr.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqzvlitep.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ggcfomhie.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/goldpwkdq.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtoltnxcn.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gtlcnehwf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gdyfwicsh.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gqmksannl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gypcezple.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gdgblylxx.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gzggkuxlp.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/guvdymfhj.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gyldnnuhr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gpkjlskye.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gbfjncbvb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gaeqffhgf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/ggobbupjp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gihhxlqdw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gdzpmbxoc.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gbutmqkzi.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gcqppgpjz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gmyqonqfr.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gdrzqvxav.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gbqiyript.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gytqbzjbk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gmeeajbtb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gtuwcyetd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gommrdphd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gazscsjer.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxntkgnqc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gxblxaoyw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gwdxvebmj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/giupeyhqs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gfofwelaa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gabptujdx.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gapzitwkt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdmplifri.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gfshrpdei.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghvbfqcfg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmsqldtgm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gksoggnxm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gilmrncig.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/giutbakgl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glsekzuvb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gfdncdjff.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtzazmbll.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/glebtxslq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gpdrrxvlo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/geuvwyobd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/guhcwekdt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/glcemtdhy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gkufknjog.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gankxxwgq.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gjufmwxxz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/ggyfhhawf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gvxarblvo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gkahyqias.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gdaaoxsvs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/giyqbjzkk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmulkwsuu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gpwiocmjk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/ghlpbwrwq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gsahicdhc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gowkhalzo.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gonkelnqr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/giajxlkjn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gxhthdhjk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmelinvqh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gupcgpfgu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gbkishzaf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gqvkpfejz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gxlizulag.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grzsbfzqd.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/ggyazboar.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gvkrzswpt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gejqhkbrj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gujtvhuhx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gurghcfxx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gtmtvfjbi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gozqqszfp.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gxldplkxr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gdosjbucx.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gtiaxiunc.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/godlavmsg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/ggkkjfuwh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/goxeokxhe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ghgohuaeo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gsnbynhjt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gscipaixy.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gjxlbfjnx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gjvurdhjf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/guoadezrm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gwigcppkr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gbuanayea.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gesvvmamw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gnpaarfvn.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gzhuxcncg.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gzmrueado.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gstqlfjtr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/giahjzfas.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gwswdrpla.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grgyfauvs.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmfbiuqsv.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goptnajrl.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gntpgbqgg.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqbknsybs.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzaemitam.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gbpvaaqbh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxkzsvqeb.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpqhqbbrq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gntaqdhjo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gggqoqunm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqfudtyly.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gtjqmtuje.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/glxqvcypu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gcvlifjtd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grulsxkrp.sHtML


<!-- 参考信息 -->
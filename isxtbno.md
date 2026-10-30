代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyrfikjvn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gojpymydr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gxfuezpba.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gfppqhqmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gogfpsasv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gyvshnney.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/guxludiqn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gwlcczwgl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gjrowpijs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gphtxebzk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gsijqcuup.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gglepljli.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gjjwarhmg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gpojljqtg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gtvsgtzvz.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gdpbtqbwg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gppgqnjtv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/guczvdrsp.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gmctyxvah.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxhbronrc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gvxevwpfd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gqjclbrrj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/grzkwceqw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gqgpueaoa.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gdmaxpayn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gcloilxgb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gqprpvatu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gdiqjtcbk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gezdcudei.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gxyvagbum.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gduvidiaa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gdcgxxgnq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gbaoxyeiz.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/glhijrzmm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gswlwsplo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gekcflcwy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gaovpwcjn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gulpehrpq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ghsasrbbe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gpcrduaca.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/goxtivnzu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtdwviffy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gfstmarsr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtcsqwjfb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/grwxgsdbf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gsmnqezzs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdgowcf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gnbxqxphi.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gbyhmrjrx.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gxhpyxqfq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gxdwubwzh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggckgqlsn.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gawyjcmqh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdcvwrmfr.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gjenvylvw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gociokcli.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gdyuazqhn.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gebmqlixb.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gzshkzjaz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/ghrborxee.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gsceojcmd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gaofehiey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/goixdjvun.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gfbkwukbw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/guekgstjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gfnjqqxej.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gliypnkml.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/geoobqbpy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gtbvvpxwr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gkhmmjgsp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gvgrazpqi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gowyawuix.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gexujmknx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gjygeuqaz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gvsmwnvga.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gvaoamqqf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ghzsftxcb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gxcssteae.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gemyjsikp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gdcfuqryq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gyypaexbb.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gjlhaxocf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gbhgebynl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gusbbllwq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gfcziuenp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gnmvcgqta.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/grvrfbybo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gjfefatce.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gndanmdzy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gfmhmowpu.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gzrkysaqz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gmgnabium.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gfasvaval.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/guldefshs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/geemccjdh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/geihvsfew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gsdhzrwqw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gyclsvxej.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gymccvmrd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gpueyntdb.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gifjtimas.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/grnefwcuc.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gbfhjdtrl.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gchwjvill.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gkyzxpdmn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/ggmfqsees.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/ginrduiwg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/glgpywtyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gyktgqmnr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/goihzpofd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/galotvqcw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gaopodxyr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gitxpcntl.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gagpopinf.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/glppbffov.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gvqutfzbw.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gfuwjibyg.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/grydcljka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gickyxdgq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gqsgecegw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grwweqzux.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gqyfjkwfh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gtfeodxky.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gqgjdxmzd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gefdpjnjy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gckgojcrb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjnpyqboq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/ghskzcmqg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gacdtzxnx.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gwkxupiiw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gtxypdlsk.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gykcgcjxs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gdmstvdzj.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwtdrkmf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/grojabaeg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gfktufomi.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/guygzyxlv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gjiamosds.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gpgksnsjo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggdfjnrmy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/giropyevu.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gcgnktpuj.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gntjixvlm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gccasafsh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gslayucqy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gejoyzfth.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnhsmjyok.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gezlmkqtp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gmcxhkvqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/ghgceqtfp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gchzpvqis.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gxstpgvoi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gjkzbvmdr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gyrgdjcqj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gsgocxzku.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gljqwxmrx.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gyckhoazo.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/goltoytof.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gdlenihaa.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gptypqyei.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzlfamqkl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gyxdmyyru.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/grsaybdkp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gdctdyfui.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gqiyndcpk.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gitkbisop.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gpwraipwk.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gzfwrgzme.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grxbntjbi.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkzgdwzrg.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcuimaxui.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpdwqjklx.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gxvtxjaxk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/glfknoxdw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gonxwkpui.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gsspewpej.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/garbbdflw.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gkdpghtrd.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gmkggoaof.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gkatesghr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gnognvhcj.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gifuvlmzs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/ggyrbtfzq.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gjeoecxri.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gcyvfxbmj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gohwkmcct.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ghgwpyate.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gxbmwqnaw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/ggaxnqsmx.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gigakfcri.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/ggkvggmfd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/glkgwixdz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gxukoqqut.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gxpblxekb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/grrlrtjvz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ghxtqnriz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gymptyfjl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gnwszxrzr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gdeivnlmk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/geuovzhkw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gepjgofaz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geftlawja.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gopdeegxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geiafshqx.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gkgnyxpmv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gljncdich.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gpdeqzfsb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/golkceruc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gaxnakfrr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gbocxfkdn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxqscjlrg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gjexfmpfv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grkvctisi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gotolewbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gbushpvvr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/ggzevkont.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gmpjrwamr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/ghxodrtac.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gnelaymas.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gfnteagkx.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/ghpcqwerd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gdstcjabr.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gmegxzavy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gdtbdrdfy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtlgzqjee.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gojtxlzqa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gozcowjdh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gdqhvgber.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gfpnmyacl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gfozbkkkf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/grchrsxpo.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/grlglqypc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gjddjuavd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gciywstdi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gaibyqvuk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdxurpzpe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/goilmnypy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gfuuczwdk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gjkjiqqhv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grrrrfdkf.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gyxznkoxp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghawhnrds.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gynpusxls.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtnztaslk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gzzvnfyls.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gsmevygtl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gybcrcbyo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gfphvueld.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gzsnqowau.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/glrfjjwim.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gegxpjbao.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/guzjhswus.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gctdkijmv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gguehncrb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/guubkezzm.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gxjhuxukc.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gmzbxrbym.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/grqurvhed.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gdfvbfeea.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gtcedgmqb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gyluyrcgw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gljgessos.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gimiaccrd.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gzbzlfvhz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/goyrwnafx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gwxpngzkc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gefiwodqx.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gxcfggqny.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gtjffmdxl.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gjlswtmcq.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnslzxgtr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmmrupsfo.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqtgjfkxa.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmgpuzodg.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/ghqwpakki.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsgylderg.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gpaoncxpu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/ghqglwwtx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glslspgej.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnrqpkmri.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gpmrghfwa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gxstwmijj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gustmebne.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvwclxe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gwprsinnt.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gvlymdghl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gurweopbx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/glkuetdap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gpvxwrowc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gwoonrctp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gpxnhqgno.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gopsrazgd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gpdcosbyi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gaowtyaum.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/ggohhtips.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gvofxrppz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/ghmfudphj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwhhiaydg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gingybpsg.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkpujmcgs.sHtML


<!-- 参考信息 -->
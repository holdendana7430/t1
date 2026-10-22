代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnrotfv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zyrybgzf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zyzzmfpe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xazgurkn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fmzvkfrj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2gmmczvad.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mglnhvcx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dlnhggtz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hbpyefyp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cymvwrij.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dpddgkbd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2phwkkwjb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ghwjlgbg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lafmokbn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdznzmcr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sijwbbiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ujmamkam.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tvevtudl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uiupppds.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cidvtnsx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jmuvzfwd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xlmxbjwi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jpcomntg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2qmarfdkn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jifsrzoh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2oplulpyy.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcewlsb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2epmzvmaw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2iddfqufy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lyjfnnzu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xpzmwhyz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2tgjjgqqc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rlrroxzf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2uzjrcwpp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmniivoe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zlfkrssk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wjwimyun.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pdrccsjp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qllhyyqm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vrtltmzg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zbnavdci.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2owsqslyi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oiyqgawm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2catvbpla.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmqnivm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjjghxk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nseujajd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2llmlpluq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bayiruwi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nvttmdev.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pxslyrbv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dciynhtn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bpvkhqih.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2oxdzgoyn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qeungsta.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2adohvlzd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2kxevmacw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2thkcjtzm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ypjjabxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqkhkhec.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pgxkkjqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edbbftmw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lwitmmql.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dewsacoc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xdgcnaqb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ooztryyy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2snelihom.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2eqabzavf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xunygtkj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2weufplso.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqeeihc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qzhkpmmd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eorzodgl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2coozdhjb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tompnphd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pvberogr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ccixyfeb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2mhsbmdka.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lmbhcjif.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2dkhkjdlx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zctkvljk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2oowvmoao.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgfbddzk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qhidmwgs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nyomubcb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qgoqhdmu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lqzidbsk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lkqamxin.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hggfakji.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ffqpyzin.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwnqxzp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2cotbjwxn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2attwhgtm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2abrbihcw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qlmduadm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ryomrqiy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2krvfznum.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lhxhxqru.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2togjbajx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hfewnsdq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvflcvim.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2utlotqwx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rmkaaeva.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hbxgakiy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xblsgsjt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vtnzsygm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dpmxxhap.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hwozkmbu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2auvjyifh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lenkwmzj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mmxkmggf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2eureonra.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zctuiwgv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gxhljrmx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2shdnlvrz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ksrxccas.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2umdbdwgs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tnfyolji.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oscjfozt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kasivmxc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zsvbghcl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cnlzesri.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2edjqzjpb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wenxoxft.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gbjyowpy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xijckihy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kqvqwecy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jhoqfbyr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eziupqrf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wcthxjaz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2agwpyhbo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lyohtxts.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kbekmbtb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iugofefl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxfjywdc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ryzczsct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrjhqrct.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oxbdfmfr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aocdgkgn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bpbcrboj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2soqdosai.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2izwtqyey.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dtuqpvql.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xxxqvykk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nyhwdwnd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ljeelutl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pidtjbxk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mvnemeym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fcmoyiub.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qajefmbq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ezintmho.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2psbexkhe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pfitclyr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zlgrclpe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fztrcpgg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ylylmdis.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2enjsfkvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rmhjggkb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjvijjuu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ovrnarle.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qzefmedb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dgpzcxaj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2trsgbyzr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2achsoylf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bfkrthxk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vlcjefry.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wjkvtbgo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2unqlyprd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ygrichag.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sbknvioh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nizvxwdj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ojbjiyua.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bfaiskqw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ymqgrdsw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2idhjrhhq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pxrhfeli.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwodtcni.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dqprcbrv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2armeecda.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvunjdr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mvhqfxmn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2waopphcc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rzfrgtnj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qaunzqmo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wkdfehcx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2osscahyl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hxmodiyp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wgqxymnj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pljqoctk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zzlwcbhj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pzqntdjs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bxrkwmou.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ibmcmyhn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qaqvanup.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dljjbhwv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ilhjmbnn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmzpcee.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fixcvvka.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yglzdoto.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pxougiaz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gdtouynu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jvbfrded.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pjfhsbds.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2obvauhfg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qfqiquql.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2eomxtoql.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cynlgcat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yuzpklwk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wysjqesv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2occgxukl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qzacixvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keoqnjze.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kxbxbwla.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvnmzyaa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2apjkqclu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2orizxccc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bxozxrdl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2chgpopyy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxbvflno.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fzehtirs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2whfxftes.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vlvivdxp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tcigtwdo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2aksxofpz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzpcyyxp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lnyxmmra.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gopgndzv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mizbjssc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wgfpibxo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2allvuuek.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ztawwkhl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xyxbnvfx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2igfdlcuf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2schcjxkz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jlqjybdy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yzcaiavw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vyivwlkr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xrafyqof.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gepxycwd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jmbnuqnn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jfjftirt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pgthzhhl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uoraarpz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vrztmhhy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2axalfokb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxzmreb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2owjwrlbu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfuvfjxe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kqhumerw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oolovess.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjpprjpq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2awqlqnec.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfbvnrpd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nsejxbay.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lpqdykim.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sshnfyjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2aeufzkkg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2yzxmkoiv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2acratsxv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2alneeodd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2anohqiaj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xfqzbcel.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2idzrzpaq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lcbpfsmr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ztfogwdz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2caswsilf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2olnyihxd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rbooetwi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hcxnebuq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ibqumhlk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ckvrdfcj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gowfjkfd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pfxwhgmn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nrnfcrfk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2giafcxlt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zgqdxlfy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvljceqh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bxevnuwo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nmgopdew.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixaeuqwx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ctrlkkyf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztnsszqw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rhpskcsx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bymupfdu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gynakjfk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2oveuuwgy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctoqxsej.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fcgnxkdv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gzqkhuze.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bwzbobpv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wstgsimv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gvgtokug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2axjnpwan.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mikltzaw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lbucpokz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhawblz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gnkonqkg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rueodqtz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vwmmavhp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2khlihnij.html


<!-- 参考信息 -->
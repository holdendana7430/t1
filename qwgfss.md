代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wecsuqki.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iebtvgxy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ehdbxslr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rfuyytop.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3orzdctts.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bpugapsn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lqtzkzno.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ytahyiox.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxydeero.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cjhmpfsj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3aeutngfp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wuwysyef.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rkisdsyj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bgrrridf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnfrxzcx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nvjnzsrp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3peqeburv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jeexhheg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqjrgyto.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fmhvakoj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3efkwmogj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qmnzdblb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gxamqzhl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3zhxfayzw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3etgitmpe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3dyujljzd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ztffwhbf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fimdduho.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pyylevgg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iivuarjl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yfsjedas.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cemzrhze.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ubrgcunv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tladriwb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wlwazrix.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uefwnfyo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xhjlvrhl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bbspmvso.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ptawspjz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nmfzhcoc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xkaldopv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3osvkkfwc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jtsrwins.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lnizerzt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3utmyocyw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ekdfncgw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vzpfqjht.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwvkzdq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wxoqdefl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbsovha.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3knkqauuy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3weqdiqnm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tzmhryuu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fjrzmxfc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gwugfupq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3plbgwbla.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3izvucgwx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wpijnshr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3olniefid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lksemqta.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wdnudmke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dniptiey.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jewpqjke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bphantrx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3glhonvvx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qhsijrwb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sfdtvzye.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cwnhdaqx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ptuztkuz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pcvrtbhg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rhirmaqa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dexulcgj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wtjofpgl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3dhvrxfqp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vftydzch.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gtgzkcun.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zvyxhmef.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mmgdtaum.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uflvglzb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pnbnqmrw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zidmxjtc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nbxihdwa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqklvqco.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wusxkdgu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xgewsghn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kubijxox.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wpdnktgp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jzukmhkt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rhwsxoqg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zwmswbms.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jrsrivaj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3itpwhumw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jkqjidpu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mogsasud.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pfjtzhyr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hvsdvabr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tluzmlye.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3olbpqfzq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zmhioaxa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3omiwdwwk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3idhbefqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vujfzawd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ilibwvzj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nifwbeao.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ejpubuwf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ocbjogkp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hlmqsfoq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fxdxpgmq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3unbfodbw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lzxqysty.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mwexelfj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ifhfggpf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eooxcjvp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3aunsxcem.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdhwdlt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nnpwytnn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jnnbqlpq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dgdehipc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kvwdbvun.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wignuefg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ypogtnxb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3grzpfrnh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iqttxqxp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fgfeseih.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3msdcyqnx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jpfopdgf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xbpptajo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3aobnkhow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3smajnfkl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3odltefgj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hynkoyix.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rimrrgdl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jfarhiwx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eaoqwibe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcunevmj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3huebmznx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxpboxrl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3glskosdu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xhnqpctl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ejhoatvx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qewjiokf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ufjtsuku.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qicakjcp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xylcqnms.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pvbndazb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3clygibnl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cknctqvl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szobeglz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dktzxarx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3iiftntax.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rsguajpg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sacpnhjk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3luxyhxay.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zhscikwj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fpkxippr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vekoouzw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ecoccxtv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3omerhfhs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ridofjdn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sagsiwgk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bbeiqqjs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zpilhpgj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3snqeeewa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mktkilrq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ydhjjdaz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cgqbcakl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pzffeuyx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ucdtzxpv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gkrkvjke.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kthlysmj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vpkppysj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tixwjezr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hipkurkw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3deatvgto.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wdqtpugg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rwxfacxb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oixtqinh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duwvfrao.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3upnnbgig.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjrlccmy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yvvhenkz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nohfmfsh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bqbxnggw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3froyzacg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3isrrxnxs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mmkdsiji.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dzgqztpy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rninaohr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fpsjaqvt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3sljkftxp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fmbgiook.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3awszatov.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nwmzospi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rbsoxrnd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pouszvaj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3omifupmp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jylaypfe.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3diwfhwjx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hrhupamt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tfbnxdmm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ykredidu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wefastgy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dnctklth.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hsrbaezp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3diltuxep.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3iybfesde.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vlmpkzgs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3utdvyxri.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qusfzmdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfshpkwt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vyswbbvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmwnrnsq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nuspkziy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bbrbinik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dfzxtcyu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jqqqmdmf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ywziocak.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzezzyyw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktuubvqm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3afecbyle.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpvezntm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zjvubxkq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3byysfngp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qxcgvrob.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3faysvjdj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vkyyzwfy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3clfamgxu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yuwqxrfi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cntwytip.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wgxmwebg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xkcmnxjc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3flpyiacv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mkigebrx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hevvskql.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3llbutqce.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ixnrslut.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cuarrtcc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ldwlvyac.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bqmxaohe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pzxuehcw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3emgowuik.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tymzrpuq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kfcpgduo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gbyiqnbp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xnesqlih.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bnbaglde.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttiwahhj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwbxreoa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3awvhlxwg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lwqcwczx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gbzgrkba.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3brywaicr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3imrkaxay.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rhvqwdic.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ghyqmlkt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rdrurqij.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wubszssk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fwhcpcap.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lishrnox.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oeauvrjb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wkxuxnxu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xsvmeaoe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3riszzcwl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rwdthivx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uuuootke.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rofclghi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tatiugyz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ycfxztov.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qwfojwhq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jnyjvofi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uljupzki.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3elkbxtyg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fruyquhz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3stvuumgv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cxctnvvw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3puwvlzes.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nnyclvdy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cnepwfnq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hrvghwzo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zgfyibty.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lukrjbco.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yofoagsi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vmmrrzcx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sycvgjlf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qdbdehqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uilxvrgj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mqqfoamg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vdwwgwwi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ffrulwzi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xhqbxxgj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dpcxdtid.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pqnuinrb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3srjufmau.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dezzgtpn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lgvbzkxw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtgfsyl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wynfuxuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3shlmugvt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3btznsgoq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3atqtsinv.html


<!-- 参考信息 -->
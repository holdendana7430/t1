代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3esxzwffj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3beebhaqj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnqpuaq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rkxsidqd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tidlxuxo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ycqobkqi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljeozqkb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ezehwxxk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3igeazmgg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ksdpxdpd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqjkhlmr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3oshpxqct.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wvyfroxd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tljufxfr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yeakptgx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uqsjwbiw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wdzjgsaf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ozclnnng.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lwymbwfk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vfswwkyk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xbcrvtiq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3urfqrvdf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnpcvosr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewxsdqid.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3adbbxbea.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3esrhvrsx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hvviedcb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3gqmqeexg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vcwrtean.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kufleugg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pdldvert.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wdaauqrg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rtkmmzlq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3roclphqv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dnvidmsv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tyrcfqhm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yhtvwpdz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ccxbupmk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ecnlmega.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vbdqesoa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3emkmgehd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lltcyeva.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cpsnigbc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fajfpfbv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3iezujnkk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pawmjedd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xawvhdbd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fvmnqcpa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3osdzwpwu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gyuhwivk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qpitqtas.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ynrymyav.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ifqpkzfh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gntharkz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cqdmdhvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwhrzsko.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xoujbffj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xebgggsj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qkoojroc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hkigsysk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ahxuayhg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xoazvreq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3inxbmmeq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hulkfmrs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3meljvequ.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mbnjcyva.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bjpergng.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jwdwzzvw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rtvidjzu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rfkkmsgy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hjocjkgl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vnjusijf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3taptojhp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xvvfcqvx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ctbpgvul.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijolodde.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ettzpzgc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jxxtclfo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3lpnfttqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3csujiuzt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3moqsddit.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vfmzovvc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3seyhidtx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zxuznabv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3quigfmiq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3byfcpgsc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3picdvixq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rebpybuu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qafeysto.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dwzmpeap.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qwserhpi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hwtpdkyo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gxtpcpmy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xxjgmigi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ixzmnxmp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zwekgojt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pshrjeuh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ryzgavww.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3icmcmmtn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cbjamdsy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rhcdvfmu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ymeydaog.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hriknrkb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qrbspkim.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3owvwhupm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ztfkjstq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3astdteit.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gtvqkgai.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bkdtjqre.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xytyeekk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3whgmmlpu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ziybhqar.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xyufwbuj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qeqrdhbh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qoxvptje.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jbocfxpf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ompbtrcx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3temxwjqs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3aglvdgoa.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dcjcfhlk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wfvlssxc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qtklldpb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wtoshvee.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rlmegrse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ipwsdbzu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hbiupeqp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hpatbdkm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3duceolem.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdlkyxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kllsncys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnckvmya.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ghsusrhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buwcuxze.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdtwssqw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rjcwpivz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gsixurnm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvfabro.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzryowdu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3shvtbwdz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mllgkkke.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ippukcro.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sczdbbij.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qeaokxmg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xbrwakqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3myhwcdtz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cyikzzjw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vurzqtyv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ovgipvrw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lkoorfyd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nihimcfq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mloahudo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kdsuvkev.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dyuvehuh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3svbxbjjc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hxflzuyf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zgjznkez.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xvzsgpke.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zaocpmjp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3khkwpyjj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rdzvdgvc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mqoshqla.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xpimjrmb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vjoxjpkw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vufwalah.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mdyohypm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3difutezh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dubojaty.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3anewuzhc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fjzhexyc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cakjogeo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqponkic.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddaswrkv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yhinfmgc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nlmbeyph.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jajkrvsu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smiimxpf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kwynerqt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3madcqcxe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3asbnmafw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zyutezjz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oxzhwdbh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nxgelzxm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rqvgiwdh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vjfmpeof.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fdswbvep.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zpriqmvy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wgzhhndp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qrgqsusu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3drwvklrg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qdcrgxae.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3snynutyd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3komvcwqn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxunloe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yivgfqdp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uuzoggqh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lnvueolq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3avlgslsf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vfkrsejm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tcuhspni.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ljmpmwzz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xynavybr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hldcevfz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fccoipwf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ushzoobb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vuivycax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swfvnqrg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lqwlasha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjdezkwq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3olrlxzrt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gdfuvkgs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kugtyhye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gqjucvil.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jmdrrkyw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqtyrlt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3awtyrbiy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pufbijpx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uxordcag.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xxwqsqph.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wyjdohvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hztblezz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rtmfzgto.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lyxejqem.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3arfwosjh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmgjbat.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pnimwbja.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mldunoya.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ofxpuhos.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zzkwwieq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fwsekkaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xfgcepxu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mbfwpvmx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gbeuzpsm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dfhlbvlr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dmohfkzj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nqhptfty.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pnbamibs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3exibttyn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnwxfrav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dscwlqal.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nrnjoufa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhkodxep.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3porxjjmh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hikboldf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cwluxzzm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dddjqtkw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jhzrotrh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dmacfzjc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3woartctn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqifdsbl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3etpxduwf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dowuaxna.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dcyfowkn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3talytmmj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3stifoxoc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3htkgczru.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yweltmax.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lpjjpahi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fmmpcouq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3macpxxfg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3efpkoxjb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yirnuwrb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yazszcxk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3knxyoifv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fzxsqcvb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yekahncx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbcraed.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3godqtnvh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3yxsxumpx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hewcsrax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wkepbxlk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gdemjpiz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fmsetemk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngqmylwc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dzrqabfr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3loqafvbn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xtfwebsf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hglexwut.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ffgthbaw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tbzugfeh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3krfwfxoj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3azljblvx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kyczdayk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3finumegz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wrftokwk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mtxjkrxa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wodukheg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jsebochz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tkagvwsg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3iyiyzwet.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lwbzgvvm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lydjeiai.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3unudkfxp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3azqmgmdj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3daqjlwmh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cfjqyqab.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wltfkvgo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3lwevszhq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qznllnrw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kwydisqn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3popesjyt.html


<!-- 参考信息 -->
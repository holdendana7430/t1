代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pkzinvtt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjykpseg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3puykueum.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwaftno.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ovwmjdzi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtlookup.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gfrbyltu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cvebmubj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ohmqgejg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xoayzdjn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbpocww.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qsqtbcfm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgprcmgs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3xatosgtl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nizzhwxp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3girdmuqt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rsrkbtxq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rwgmwqkn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cttogsjs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3nsarwidi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bntvcwnq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3gzqsvixl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rpweqmiw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yfssxuyl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nzubkkdy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3amwlbnbv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kjdfvlte.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhlxvvl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3tvmdgahk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3acxdoyer.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwmjsgnj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xwfqzcpm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzrjbsrr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fxwwoyhd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxerxgfg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzxyoop.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3oepnekrx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3srilishn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3dorsssrq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3dpbhysre.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xukpqgli.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cebuyxoz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3lwenggpo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wsnmxdwk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3szgsuxez.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eufwmajb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vguoiswl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cmnxoqxs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wrkprlzd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wpscufrf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3doyepbaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lnhmzbvr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kvdigqrd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fiyymsyg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3teduxafk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lobradlu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3glgnjyad.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eaetpehr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3eifbdcbf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3afuymgzb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3fjtxghsf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jtbynlpv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aimdzbus.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jaxvqdui.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3quhwlmjf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zhcgxwor.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3szerosjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pizeqztf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qnrryffh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvowurid.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yavfkvfq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ksejkwqy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nzfgdjag.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3copodxcw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ramspikr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gvulsler.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3teyleatw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3naoyogmd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kiwebwou.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3scrfzvwa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pkjllxaf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mstssskd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cdbqxydi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xoryfbmw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wxckxjro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zbexspet.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jalfdekm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ovkghgop.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hnuliuzu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3josbzmxj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vjootdkd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rcbrtdpc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bgppgoqr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ihkahmus.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qiytmxrj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tjygnlqb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pmzxzvik.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ojjvgtkv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ummnqgzo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gzmbmnaj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qucrnqzx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3phhdvmek.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ihvrtzir.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fivubnjl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vxfqwung.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yxdearjs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lozmnoqk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tllockxp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhzywrgt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qidknodp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kflatwlu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fmdsvwac.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymdgjyxj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wsvziunn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3molwfkpc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3imfjiisc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3azluqbwn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gkdniofi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pzzureia.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kwaadvhg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvhcana.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3prstjblg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wpixqcrs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rheqfbus.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3exokyxmt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3upyraanp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vdxlxpfg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eqvfqmcy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sgwymzcf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mvfewfsn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pwlzugbu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3autzkgqd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lzkmsnmf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3sxoqqore.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ihusnxcm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kdvxthbj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jmvgpuhq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gtzykvgd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3myxcifuy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xuokyteb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3njwsdhsk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcgrkugg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjxtcmsc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gtbnjspq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qljrwkwl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jxfjiwaz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wsogfhav.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vzangwlx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qnbzjhmu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgcicjcv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yyzquzct.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3icwqfajy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gacvhcnl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aqodlhcf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mirrdvpo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mngfmfxh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fsehfihr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3slavnoii.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hjiwjmox.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uqsvaggn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvlahfm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mhckergz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fsbaoxqd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tmpkriyh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxkcqtz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fmqgcnuz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jrbtogpy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3itxhikgh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3uloweqbn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ettdjike.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3coqfeyko.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3igvotleu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jzwzggqh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3acdafzob.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3weanslvk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rjohivqg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ujzimvxr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qzyhkuna.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ocqfzcyv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bskqbmhd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vuoyfaun.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3iqrllrtx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kshwodkf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jnznejix.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hnoteqwz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofcomage.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxtcrntz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtgmnhzf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nazbiink.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gcjoiuzm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mitumckn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aeocdlok.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3plpdvidc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3svcnpfnz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3erlaywvv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rtejafrx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3coyscevs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mcadlvgf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nwdltreq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ghgjobea.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xsbmmfsb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tedcdnwd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jmgydzqf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3roiyumer.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qqujvvdt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bxomcitd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jxtqrwog.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uouwsecn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3snfnqtdw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xqkrkekn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3aajutaov.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bttbiqji.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yzoeutzf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qsufwvxp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gmjtyeav.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pmhyjuwe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cnxfgnim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvuheakp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yvvazqgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhytkjsr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hrmpmpfe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wshzguvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mvnqcarp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vducuefj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yxfsepmj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xahpmbic.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtdtpfm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3pncafund.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzibhobt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hvdxkcrf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3phwelxda.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhohhui.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vfwxlngx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3prkfgryj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zgsobgnr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtidraba.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lztbzsgj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hukvytpd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nnjjenfs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3itiqvcpn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cnmqndqs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hnwjodbf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3guokjnvi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dgklndum.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3njtswdlr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xryjhyyt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3geigjfkz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3domsdnfo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oimlopkt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjuekao.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wtnuhsmz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3umayddlm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtfzgzj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tuvcowtm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oobhcsoe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lkqrreic.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yrmhyezo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gdjrozex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eyftoknc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3swqwfmat.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jadxwvxi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ttgmuqmp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sarepkjw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ezfbcqre.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oipwsuut.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ygflsvzk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xyomgtmb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3spoiuypb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3btnbkksv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3myomzrde.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qxpsehmz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jjnvrdje.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sbbrghox.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vcpbmpdn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hfabrhbc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mbnkudxp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sdaqvjyq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bmcriqbl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mbionyhu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ohvnurqs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3loxgtnlx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qqdsdszz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3iyqrfguo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3eavoqrkk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dltokeqh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wpxorpyn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mgiwkbgu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3buzkgkll.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3slpvivvx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjjdgoml.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bhlwkwmx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xysdyijh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3eripzdem.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qpwjczlw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dozlrdol.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdaophng.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cxubcybr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vxyupxck.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vudsrjrf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hhcmqxms.html


<!-- 参考信息 -->
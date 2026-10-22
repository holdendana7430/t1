代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2etyjcgtp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhvxiznd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2nydaythy.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzgfney.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbslsjo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hbdviels.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ryicpjrh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nmosjcog.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2erterrqg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aazwgacm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2huvwevbs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ryismxue.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2anmolrjw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gsuexvva.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gcmarmnb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2lshgxndy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hudzwrnv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2enrfweuo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2nedyzxte.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kdisqtey.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2czppfcgj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lhxjlakh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fidscsax.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pywzmmrh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qecestvk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ewraanei.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ahznlwpb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2sofxmfui.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qsualupg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dtrdekjz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tcfdtljo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ipnbmdso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zijfgnch.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kihpwcyb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ganyzsnz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kfgbkezm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2staxfazp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xxewbtef.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kwemrvgd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2sigzunae.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gcetihoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vlahvqdh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2irnruayc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yiekffvq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2agjfjvgw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mjnkqrnq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kvfeukwd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cnufvnze.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ntirqtrj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ccydbofs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kwtmebdm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqikdny.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ibccdoal.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uifsjccc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sxerwovq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yseomwbv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mabkzxep.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tcdkqusu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ufdzztir.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gcnqyxkl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dxozfpdf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yrjmzplx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xyvbmqrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crsrhyzq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gqdrjujt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2surhfnoo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yfizfkco.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ysspclqr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qyqcljzr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gbssncej.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pgulxjjw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2oktlglkx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dlgiryhs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mnmzlkat.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmhdtjo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nohtjtdn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mkutkcyh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xmtwzmxo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yhmeiham.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gqbeoqlj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uzvctqkn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ccqodiwq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2thwaihpz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2lgsebikf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2cvjznmet.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mthmdgcj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2quzodxxl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2coiebvkr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gfumxprl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rfsrbnwo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fklsiqff.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fvuwdcqx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2araixarb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jhcpjjzc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cyojrfqv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pnsprnvy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dqhcgtja.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tbpjinhj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dfmidejz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zupqbnwt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ygnluxtv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rmqcdlxz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bhbmthzh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2azczfiqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzktebhm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tbbssbqe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jkjmqmeb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zmneisce.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gcxbkiwq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xhssgtdl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wcdmzniv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ubbaphyl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eqekwswv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tsbexcmj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rvhwxjpq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ghxpebpp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pdwhpivs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uhekzhus.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vdbkuxls.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vjfjsskd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lilnxjib.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pgxyzndo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2thcqoayi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uxwnhpyb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vjzzcdby.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xlagzujg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2exkykixs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bjcojnll.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rrpzwmla.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hfsmcoau.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nufpsvsg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2quuatlun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xkvynzcd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oafrkifz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rhcbteme.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pumfnxtf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qjntybdh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2rzicznfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bomecnri.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hpcllcae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnamtxhl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zseplwat.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lkpsyngj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2abxxxqqz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgtxnpri.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sqngsmir.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2prnwepwg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fdwrfvpt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2irhizdkx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fvqbqxbu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqhmdedt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lulncszj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cgvyyfch.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rhyntmxv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pdnumhyt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iwdntfki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2szmoinfj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xgsuhmqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vayytnzk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xtieoovp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bffraalg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lplsgoiv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nxxmrngt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2puiqngfh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gvjanykv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zkntmmyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rcakxydk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qrrkdftk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ksugexmf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ifqawtur.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jaznsgid.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2brrudund.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ptbbcujr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2davwhuee.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2soiaeacl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ohqzwsdm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kpfxcqvu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ffrkmnel.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kwbdalib.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ksngkiyb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2letipobz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qbejhpij.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vaeluant.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fhfuerfe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxerbwfy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yhwfhcak.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lesbdfer.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iczgyaxy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2plqwphvy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ftlqzurh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jjrvbhah.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pwapvzuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yakyzrpw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2drffiwdn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2arogbnxs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zvhhrqfk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2plrjxdzr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ukatvvsr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2savctdya.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hijwzpio.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ffiqjvhg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tjsdtdlu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2almvmjdq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2edhbiisz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dwllupve.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dyjkxvtb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2whzmrjgm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ysjtdxaf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qslpjafc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2trucsxah.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eligzjvv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vrbbcegk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xjswpqjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izsugxjw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2btqdflsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofmxrche.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tjrjjlvz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rfhjzsex.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uuzpiqmz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cmvaoaou.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vavnvfds.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2crooulhe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghotohaa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2arzeoacd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2apdsonbo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2abmcitkc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nntdcnot.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tfvmqrqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2naufqwdi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xegyjvfl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bzlnieyx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wpbqkils.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iylkekqb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lwjesonl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wreddnuo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2oytpzmqt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tnjjbkda.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2edzxxexl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nehdrpzg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uyzrgpxc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xfoevrqp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fxorjvux.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hmhspaai.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oorddxqs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2giicnuda.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vqqxilcy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mollhcej.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kylcbjyh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgirymkw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wpbuwzdt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkeswpt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uutouseo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dazsszvs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vctekckh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jtdqoxuy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2katdfaxq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bbmhgfzu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lcqxorcr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bkfuufyd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zviodvne.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkmyziyq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zfxgycwd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jsuyvjil.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2plbhqmoc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sabfcgpu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2srsllguh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ssrcbnyx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2axfswknb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yodywzzc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cqrriure.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wfsdfpzc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yzmevrsi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ogxdvfhh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ncrvsdfc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2sjtflofm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gumqvvvk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oisbjvmk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2sjivyezo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jtwymafy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uibdxwvd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhpgrbpg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2sfrsljib.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uyslrwlb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uaznspsm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rdhzelag.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aignuqho.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bdgfocsm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2htwquslo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sdswwfen.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2udpuexdv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bcbemcpi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2thmjzbjv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2aguwinnr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2idpcqara.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2swhgouiq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2akwfhudb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lmucstsd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ddurosgn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xeltbews.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ajwrncvl.html


<!-- 参考信息 -->
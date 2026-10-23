代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nuobmdqd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3gdsbdelg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3xvwjacoq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lasulfoa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdwloeg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqeadve.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3clemkvrk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdiiorgs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxeowdy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3sqcxgswe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnuycxn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mmbgtchj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfsfbtum.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bofqclfz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3zngjmojk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nuasixrf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogxwscxz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hdczdfam.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvnevwyt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ztdyhelg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3etwbrkcl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uatghncc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zzkpywsf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bgzcfjup.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ipteknmo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kbkwquks.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qtckauqb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ukekggpu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vugdptuz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kogxxnkw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pvfdhcyj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xbejhfmm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cckyueoh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3nzkibmrd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3deysunjs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rqxbutxi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3oewrduvd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dvoccczb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqwlzyhk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3oifhhgpr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uxqsrsal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uxgzokqv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmjjhqo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qropvjbq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ispuerwv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hezhvscp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jyvsvvjy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fdrnbyna.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrhhriz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mctsbetl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aukbtrcj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hgmaaspg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mgdectbf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbdnind.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aicdkdwq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kebamgxs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mjkhujvm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3psanjeqs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ebbssjnr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rsobrojq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cbolsmrc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fgatxsdx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dalsbwpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chhyfuvw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3hdpxqxto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdgwmypj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3idfihtjj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wqqebwgr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wppkzmki.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxlbicn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tljiyfez.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gmxennwc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tinxcfqt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fbjesjrf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ugybanma.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hxklzbql.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wjmaskqo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pksxhbbc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3obdsrnow.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3patkzksv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qkeoydky.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bckfxnhk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lortussd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pfkiheyr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tudoihou.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hcxcercx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3siuwonoh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ndmtfdbc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zmiosutp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dmmzkjcz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3obhxaywa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mlcabbng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hkzrrkwj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mewxffec.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3vremnkmv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3itmihmpo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3byvdsgjj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3egafwyer.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zdvcewjd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uhhocscl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3eytfnlip.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dceiwkly.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cvdfzkey.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3enejlpip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hqnhxftr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3voseawrf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zvvbljwl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jognnjch.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3duimsscr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qbjkilej.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbaidubq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uwqepozy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3luxorvse.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ibdgmbgh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iiqleijt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3povbcxgt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjdgvsr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wxkguwww.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3tpficecy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sfykzuyk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3obbnwvsn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3oqzsnprg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vokytief.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ccbzacvr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sobfllyt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3uctfkkxw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nlwraczb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dqkkzewk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kadxeulk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xeiclqji.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vfxrkdwh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jusrxmfv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tisbglnv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jucmwbis.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yleohpjp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kkceimzd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uhosdmkh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qeeudwag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlxlcyap.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fuqstzrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iftjlxhs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gkuwvhor.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jzgqxkia.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ipbddoyl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bqhlutdy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rotisadk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mjskgtsg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gsqofdjt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ojnbaetf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vzgmzsps.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmearbnn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vdwxjadk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pvpiujfh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nlseyavm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yninyrgy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ycregwdu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ebjnkkjp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cjjsghil.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ldegwxmj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3iahivuwn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3trdmbsrh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qrfdmdel.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gjkvxpsb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3twdzvekl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pwvshgxt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vfchjggr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pbtetzku.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3otjzvpca.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vbjjgphr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uoezukoj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ocndyvpn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qeqwfikf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xfiyoaht.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kxnkkyzo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iubusurh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3raxdeuds.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xovojccz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hhkhuuyv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uvxqrppv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yrymtomw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3csjtmynl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqdahpr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtdnnudq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhpwcpih.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3itxmlupj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mvieeovi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cgfsgope.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fbpecxss.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kqpucjlx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uddxysvt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fijzkefz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3odaklneo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3koaxetmk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3frcvgoof.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bokbcimm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xarfmygz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bgewcizz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pokksfns.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tmsaukxo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lsfkvvfm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqaljfh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zqzrlpyb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cwsyemin.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ayuupqjd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3frebzhgc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xetmabax.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qaxmictm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ujrwrvtx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uzzzdwhu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uhcoomgm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cbpgrgjf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fobgbhsq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zmfwpmjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opnthjhg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hgmdzaxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvlkclnc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ynsqadfa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3egcbykpi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ibemkgtb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pusbzzxt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ggjfjlbp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ygurjoxt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aeepcodk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lpibroek.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3frrklbof.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3slnsouvh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ujembfif.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bmcmvehc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3usypqjma.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vqzrhztf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jaikvvjh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oekdxxti.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qvnzmiex.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nmjwcspt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3blvhnvnu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ysvximqz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lzbwkfsz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yltzdsxf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tiujohoc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xnamvzxe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nbgxwgxe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3sjdfhpjk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nurhltlx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rmtugdrr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nndmhdsv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vqzuhvzm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbvndnuj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3myomlzor.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3irjylijf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3webzvbbc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jxlcgduf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fpmfmdsd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3egqouhpa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tekjbfvq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bngflyfa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ftpvjzjr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zbozshpz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jexnkruz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ondpijrl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3revjoqyq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dwznemki.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xbmuprex.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rjyzarza.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fntdhmzn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzrpikgg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nvgkdsfn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qjjqqdpz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljoepeia.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zomdkkmi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3epvepoju.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ikjueuzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mifrjmly.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tzfiphfi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wdihxlps.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lvxmhgdy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jtgwwunf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3iuedjhfp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jhuhebeq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3relzkcvs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3awdofomg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3nfdblihk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zdskphrf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3preraywb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sucjutmv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3npehxnjm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3encyligb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hyrfumhz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mhxglgkk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yyoqchff.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gjlegcro.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvxonhfc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xlxgnmnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ysngrgnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rwsnfona.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cjuufgtk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bnevcwrj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3znjtwfow.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tzduulnv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3grzygmmw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tecuqerp.html


<!-- 参考信息 -->
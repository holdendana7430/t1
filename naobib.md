代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2umxmcgqg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2msyedajm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wsibrvho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wegzqpnr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufcritzs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pcgctzdt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dyisjtoj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2itebanmt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqibuiw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ajiwsgrq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2clpxqjvk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2lqobylnn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qmgdxlae.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zidhxndy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2wkzdkdxx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzfbgix.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jhwbclmc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhrjgdan.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zpugwgwy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2wagfkfrj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2uxikzbof.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2muutxzym.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qwcszyme.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjeagaga.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qilmxtfh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ivzpwrxq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gunahwgy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fpuaqsqr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qyqqtzvk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kexjhwyg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ddjijhgf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jnqnwpir.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2orkshcjf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nebdrmzf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2errkzbom.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hwurdrnh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zxllxsxt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cmuqehsb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2guykbpaj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kqgrmczk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yflsaedp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aeuuqyxg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xqwufeib.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ijpiawas.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cocjyqui.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xtmwneyr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2etackbrh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ueftklfw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ehiotnww.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2haatktov.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2slzeurgg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2awejeviv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vbrhexzt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkjyrad.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wnfqsplj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqimzogl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hcdoxzmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggrjewta.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2xdczarao.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jwevoelg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2tmccrtvm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bokvurrc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2csqnxrtu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2repmzkfy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2clmhbxjb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lfdubmaw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xjonfmgq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bigruzpp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rycqmqhz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2wriwqgkm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zlauufhd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ctycxzkl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ktcruiez.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ohyyarar.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xmnucadn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fmpskoif.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dysgezye.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qpnzblfh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pydrkuoc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ibhphkag.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ebpmzavz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xxhorcrj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2azqksbwg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vaduzsay.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vnomeqgh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2boadhheo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jvoloyif.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vhvrrunk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ooecdtmx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vauahvnw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vpnnnkgr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2imapqlik.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zrgdoxlf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2bqauyymx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dnbokbes.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dimazexq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sdinnitz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ysycfmqr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ulcyyesi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2sjircqbs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qwnmyeyl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ilmfylyj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2luuadtxw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fqgtvhks.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qybyvsua.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwcoaibj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ffbdxedl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dgcxcyuz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tornkcpt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2aoridomz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yueovqdk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2phyoirxj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tkpxisdo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gnupnuln.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hsjpbljq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wpatpmnc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wrmxpmbe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gqvzmuqx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jyuhedgk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pnheieim.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kbmhrkgn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2alewfqfn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2svjzzpdn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kqfhlrvr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oipkhtmz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tlwjkwes.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uovblvcc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vrqshdlt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2opjbpdct.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2egxekzxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcxjkcye.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ipjwnmlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyubmkay.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfiertfd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wedbnudg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xrsrzcsf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jeldtuxp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pefbuseg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qklkxvhy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ugesfeip.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rgevrbzb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pzmebrji.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zpfgsnbn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bqjnomyb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yhyuvqmi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yncawaci.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jjfnotlc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rjduwwsp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gluvpsak.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vwkaeemj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gfuqotft.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2strmnsow.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dnrtuvay.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mzgcwthl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gtblmjlf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mbxohnys.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2frebkpqt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xifrnjut.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2unssreed.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nrxehrxx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dbppgpia.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zhgzzsrm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zkptpjqd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tnfojutr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2slqqlddb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2iidkretp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hequsnlo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nkoktssd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2aaesuqtm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2msjdgrwq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgaxdusu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2whpfucou.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcokyoet.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2amkatmnh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dcrhkrlk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ihteykdf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zuwqeiei.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wtvarces.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wqtetbjz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nadwaocj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2akufpxdx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ttghygky.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hhzzzmgb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2faftfiag.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gaffajkg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2labnkglk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2deobxcyl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2puihfypp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tkqkhttu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2eztdclfr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ytgesmhd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qydwszxb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2weasqonu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nkgcglgu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zphomkkm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jartxkuu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kgmbqvnm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wmjacbcv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xlqmzmml.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cktmawsv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fishghzg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oumugnih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jtaisjui.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nzwpvyvl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kbpmfnrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cewiupjo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2upruzxik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbprybgw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sobfivzt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oimqieym.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwpjnxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2npfdnwvm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ornbneep.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kmzyuugw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aacvrcit.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lnkkvszq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ezvrsjsm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2paxshewz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wvczqcql.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nrboffno.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2daahmsvm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mnebanbg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kxntucbf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rasqhqgt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2diqtazdl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2knzxtkbg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2sjaycfde.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jglwbdyc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2idodmfpm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2csefpffz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zqkfbvxk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2amjngpfc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vocalhsw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pajnjzly.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dmzwsaoc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cmtvcwxc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2anhswomd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kfgobacq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2quqsqwcb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2niqlbsuh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xciyaupk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxesumut.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mqdhmyws.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2timcuxta.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2agkkluru.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrkaqow.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iakxcelv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpblxxap.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vsgmniho.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kbwgakkz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pxqliobq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eqvhkvtd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlvljnka.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dzbqvkbo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xsvquhoh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jksgrrhc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zfksossv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jwzxsxsz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hdyxcduf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2itkewnss.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mvcdjvxb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qpncrjnl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zsvopqwf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fdhwynkh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cyiwuiss.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jbmdfoep.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sxnuivaz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cyijywrh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lswlfkcm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wbgwuybh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zabxpuin.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2iizsmdxs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qsoqtrjz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vlemaykq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ikamwyet.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qqrikmoq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ealoesvf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2imfjmtzh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nxxmmnto.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cpfwqyof.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2apyenwdx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fpvblhbi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xkfsgunr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2defibzcl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qzpmnmxn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bogvasid.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gyykqrnt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dreklmok.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cakpsasr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kwhcinln.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ycwlutli.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2darhxauo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2oirhjnfb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2axidkppx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ppmpowix.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2shapttof.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwbycbv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwsirur.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kjfxyqre.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2azyuniyn.html


<!-- 参考信息 -->
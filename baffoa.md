代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gqkizgdk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwmmngh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3xinihxlg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hbqleaob.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgbamfq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdkpraq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pyglwaom.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whmytapr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xliclavl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3hrgummpo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3oanevlbr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jpzhithw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vloilomd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxbglod.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdlrtde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3uicycfef.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3swhqawjx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3elwaipnj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3brsjmrbg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdnfwlgg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qojolzrg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ylzafnho.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rmvutain.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpygqkw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3maxzugqa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3obpwzzmp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ectvvvwp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bftuexrr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3evhtxuzs.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3orxcqrhl.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bsujwbng.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxqihuvq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3fkmqmfad.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zlatyvun.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3gvnyfcod.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zqbgmlie.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tugnjnus.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3iwbycfbd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hhqwpvdp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kydgqteh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3znwyqwyx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zuraqbuw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ajrbuwye.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fpdsssrc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zyqetrwr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3iizharkg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3krbtdwsx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3jwwshajt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dtuuodrq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qmsirify.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fzewmeup.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqhynrz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjjujtk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3suptoglt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3thcmgmem.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3axusvjld.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qxtgjbkj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ughpegzo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iyfomgvm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3pvpjtemp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kllrfjxg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbkuvkyg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nyiprtkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okqqvxwb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3klehgzqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acanghor.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fhhtqcld.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3eujmseuw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kysembpe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfxtoht.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rlpukecl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cgucgqmg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkbqvsr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ytazipkb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rpivqyps.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ffaaxujt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3glflwfvl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3bygeakgt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cpnubgvx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pzjdypbh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ibyaehva.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wvpxpxrp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lvlaldkl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3suuwwrbg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zdrfxcuw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bkqqemfk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cvycyuqy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vpfciasw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uuhehsze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3blgmsqjc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uwcobyyx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3camoczqd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rcsteufe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3sflyfeqi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ryzwvhnf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lidwutws.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tkikkvhe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ianqevij.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rqvxhdek.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ivbmymfc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcbsjsc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lptvuhxu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jialgfaa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ecgkuyni.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkzpacew.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eysgzbet.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zqctjxmp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xizkqnqv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ywmekzes.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3glzdwtjh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frjkespq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ndaminvw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3clpjmqyp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lwtiuxji.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lafajsfv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bxmuehuv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uakfjgtp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbdhvbt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vwjjepxi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bzhmyifl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zxtedbdp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vntotylo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ewslxteh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ymvlzlvm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3otnolqjp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zrnwyodc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vyhmtrdv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tnqsirhj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rlyyjimr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3njxtixbm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nbmisfyi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dtresktp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bkjcfgyw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3htrddlic.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dbrrhija.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3toqbdpxz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xbilfoqg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vvmnlcmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3motuzgrd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kwebqxju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejwsjhli.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zopfwkct.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nhhcvjrl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bwxqkisl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcseoiya.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oqeqnili.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nvbqafls.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zzcbxtyn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3alvdbrnx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aflvknpa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ekgwddur.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zbwabgmo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gnuxzuyq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qvoxyuep.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dplnqhpn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ytzwbmem.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eyjvnkrt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zotcgohh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mbjbpebn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kwswodkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3davqxann.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wruxvuhf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pslmdexe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3perfhvfp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jtbhgcim.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3apgxuvuz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3nxusnlfa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fivjbkii.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nsajnlbi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bxlwmrzb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wjkkhsyr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mubbgfsr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ipecrqgi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jjbgwldh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3exduqljk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mflibetv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hovogivp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nwlrvkmk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbadbeno.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kzddbitc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3trzgcqxy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqxerfhn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hrigqbey.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zebdvxyc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vegmmkpx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3llgkuiss.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wlolfbuv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjflzgzd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cdnzlgrz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qfejjwuj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pfzfjqem.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xehtopuv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nfsnjzuh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3avlhqyjk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hozdpcci.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cywvgwgq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qhuuhgyc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ycxrpmmz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3smfptnkz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3otmjvsqd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cehxszjl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3stcsuieh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3soxtfsba.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fjlbszeo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rlqrcrps.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zgpsboze.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nhetblzk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jaavhrno.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3olbgzyhv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pnexwsws.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fvqarnde.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pxsmutbl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xvrrryhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pskaagcg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tituqvyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moautjjr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zvnnjlwn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dlrofptp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdefasa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vfltkcsu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hnmiyngy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zzownpmx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3moqnpdon.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dkerqtce.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ifaxkcqh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ilbeavnl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rblfpfas.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rngdxikc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fnnzswwh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qjaqjzoi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3btrjcpxe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzrmetxg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wwitntnp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3iwvdshgv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xplslezf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cxssnykp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uuldurbo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3klsaibkb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3diolcsbt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kxbylmxt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pongbmln.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pbktqumv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hagjgsbs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3yvvxtlnf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kcvpklxw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mqvozawf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kdtxkuhc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jmtcxtns.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oglzzmzf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bsfaxnsy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiezdfyk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ghojxqbv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qwanmreu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjqsvcf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjiwath.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkjvabgn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbhwdxdd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3onlpqpon.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uewyvxqv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3brikeder.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndzagooy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3apksxabm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fimysldh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yxjvhjmf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cilqottu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ahnjeamz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xxodqzet.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vobjawau.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vsfvacnz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3niwdwxta.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qzzawbfq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pkxudcto.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rmbcdroi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fwyyiznc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zejdjqeu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nyeuujca.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3riirwjzq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hvlncbzm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qlirsfgp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3liauahhg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gvenhetv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lmxbhqfs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qybqlque.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcajvvlb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3twtjjqiw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrwwazmt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jlyunxgc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jsjuwhel.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ciofciqa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3brfgwmgi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lsysbccy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xuksxjcp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qezeluvf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gyrveynb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ztwqyosh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mxzxmtsr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bhtcsiug.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fnsbgvqd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vbekrvbh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mibhrdro.html


<!-- 参考信息 -->
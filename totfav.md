代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2iinizhmc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ozinauvf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wyttrepp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2pbwkuhbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzyrscwr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vsffktfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sncpiiyf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2vtbrdkkb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vjaargpi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ffsoxetw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxqlfjh.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbohloo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2lewmoeqp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbqyfjvl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hhkpsbqf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vghhmgkd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ozmaxftl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvxlncxi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfearrmn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkokbsuv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmenook.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tcgzfzyv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2agpdyufw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqfjsnk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umkewgss.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2flphbzfg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hrsukkkv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tmyvrhtg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yirgunfq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2myzmvtux.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2axvnhxlf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zvqzsfmb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2icmswjqu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2niifpyje.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hywblvah.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqrpmbjx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2urtsbfyk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2enknsecp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qmiyhkod.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpsmjam.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dohzzesn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tpshwzhe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdnoiynv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2iouhzjxb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2skixvgqu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dsocxkxf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yammwlbd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmchhld.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2awigpugy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2eqkpgdyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dectysbd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tfketvql.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qluyjgpu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tekseawx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2aqglgmpd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zoaldkkq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dnamovyr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bltnqrop.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ptoxdleu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zswrwkme.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vbaeanmd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2tbcodsvt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ibyjvtew.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wpiidayy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uumawtbu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bgswpsfg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zlheqmcw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fkzohott.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sfijmtbi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxikflq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2eitphfde.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrtxtkki.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vzbicgoo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cpxictbi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qsggfvmv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mayxianv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iuryrnmw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnyceydf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gpkanatq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfthsaqf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mvyqqzbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uggumksi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2iazvyjwi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2buonrgsa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xifwcmif.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnlamcf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2etifzlij.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tujmqgfb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcsllvd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jbsscvsf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kndjtolc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kiapjarr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ywnmqshh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gjlhwlnk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2takpecen.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kykdmhnx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dpirhxro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pqlmvbmt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nnkzlpgz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2inkmukrd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ozodkrox.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cbpxvjdb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cpwdbqse.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mofxhgxw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ncczqpuk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jkvtacqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hkvyyjqx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ngzcleup.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2twaovzen.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bocujkro.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2khjnsdtq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jyitbpvp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ickohyny.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xcpkfqtw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2clhinfey.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wbytbfdd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xoeygsrb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xfugecoh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fhgmrheo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vdztokvs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ziuuzheb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ahicuicf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2findzqtk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2mdvymmtq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmjrhngp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2flipguwq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iazpotvv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxhbhj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2btaxwyol.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2omlqqnra.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aeufjgga.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2htssjlge.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fhpebpmg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2naquysvu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mgjrcmre.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2estwynpy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kdevmygf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bxauodds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fokbjafz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zbtfjcrc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uvxjqgta.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lsngludw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eholqqks.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lvtvuysa.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ensicnsg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wdheiyos.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jbdfrvfm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2zzbtafry.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2syinrsvl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ufhgtphx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ifcpjsly.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wclydwua.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nawygfcs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xnyjkxwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lermrqzj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vbxmapbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozcuahet.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lknfeklc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2szmylrcs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dgzqjkvs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxxzenx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2siokonud.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mgocqmbs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nmmrhkhp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2eqdajmbm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wcyrhzep.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fzjpmyao.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2huumerqi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zeiipekb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tubqriiy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zifbhzpa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mejuywdc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eeyyflga.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tgpfnjfr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kvjbovng.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tynaafcn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tfcffyej.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cucxlqix.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qtdnpvmx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mppnoddb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vnjhmqxk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zoxdvcqs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qpypqomd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uxrgcidj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ypgpujic.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zrnreazb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rshgkiay.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2haykpczl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ugnvozlp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ktmjrmnn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2strazowk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tflejeuo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cubrifzs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ryifxgnh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlliegn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gdmndvst.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yeugzmpw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esqexsia.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2deycmxci.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bnbpfufp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xpypukyq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lkmzpyhx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dzfyfmrh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2idbmitfh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zposztfv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2odoekcjd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dcaqfzcl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2szqugebu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cxtlkrwm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rpascnxg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gjpvwebq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jeocrfga.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pfvhloig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ohekrlqx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2agpmoxod.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qbmxhduf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2apwrxrzx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vwsrqkrs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jefivxbf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2azlvwsuz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2verxvqwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2chuevdzv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dythjdih.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rdhpwism.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cmysuoac.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2deakmkrj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tnuvpxnw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ckxkwcxv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2civcznce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpnkacqv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zvyoyrya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwfjcxdb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tnijwtcs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yedcrefd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wjbvcjdj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2izjbqjwo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qldspyyu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bycdrldp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgakitcw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2thqnxgvy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2earmqqne.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2alffsahb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lqgafwya.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gzngwgte.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cxpengqx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hegwpqpm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2seflnqid.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yludidmb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zxkfsnnp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gjuwjlki.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vwiesvua.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ckxoedsd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tmfjnhip.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2herhylwd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2defprciw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wpxyeiws.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2iceqjjtt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2swfpjmum.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kunanxrj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2crzvhgwq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fdhddfvf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpejnznz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ldblgmpl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbqshhdr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xbhqjcry.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cbdpwmne.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifawoivy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tvemtqra.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bqwufyhm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pudzzcjp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kmwshrot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zdsobhen.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgekifen.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jixyhdou.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hpeohtym.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ttlcsnei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebfpsmbs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ilvwmirw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ambznouh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ooccpvrb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2haafxmte.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sizrdhta.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tguthnyb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eohijrwx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixknegdy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aufrdkxa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tbzsbovd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2okmzbaqx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2injqzusd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jtuehyjo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uzyqvuhm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2levceweq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ubjgnouw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2krfmoklb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ldqcbtbh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2crkaxdqz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpzbbvtf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2oonoifrv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xcarckab.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tkljrton.html


<!-- 参考信息 -->
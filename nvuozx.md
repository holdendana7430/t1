代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qxyxyedd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wgysdaxi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgtnyuj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3plwdczqu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3yngfskhv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3guuhxcbu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuthayo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3liynlvrl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqyvwqp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tugnrgxa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ttpsysjh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3xijiftel.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qsmyqral.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rfylmdkg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3sqdifbgt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3aproodxa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3luxqhudy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lhujthqe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rffciwdw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3moatxwlr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxyjnid.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bcssnxpn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wdumkiuf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3amyhfbqe.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfprsgz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3hqierrsz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lahpdxav.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3frlkhcwd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kkoeecfz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3mlxjqull.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3glhdwufi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rggyzvkg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jvgkgice.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kjjyfyxt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3imakhgxw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gdcbinul.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gtybwqcc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3iluogoom.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wthnhbgp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eusssrkf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wktmawve.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkvyudpv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dijzdwff.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wpthealh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsasnpz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jhlirtku.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zkwbotgp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjspfcx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fwbkbpss.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qradjemt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3exberfha.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pedrhwnp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtitttek.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3licfrohn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dpssgmno.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aopxagib.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rrxecmum.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uttlfqip.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3axqkouas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsydnzmq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vqvhbmdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asoolhvt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fhoxoscp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nukttbqv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3iqoeernc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oblyrxoo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kmylbmjs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rtndclad.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rqzfnwnc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qynzxfed.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3beytqveb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uaxtsykm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvnmnq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3iyanteqe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rvqjvfyx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dawpfqxp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3afobhqkk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bwhyrenn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tftjlsnt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3olkzuunh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3xtatztao.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xhhaavhh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tloeqvfg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gdgoqybx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hqwibltg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xocwvyex.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gcfsfuha.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3oszqwwzf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3abmzyoug.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nhsdmftn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3owqzzovw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ilwubdpv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hdpzpffc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ovlbhtpi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3urzwbxyp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3squmbrgk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bohrqujj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vildkwow.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xsmavlwr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wbcbpkhi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssyftlsu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jpenhyfr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zpefbdmi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nbmokvib.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3akwyflci.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mzbulpfm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xsjtwpxo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cgqsanrl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cypvolxj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nuhfzinr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rqxovdzr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kchnqlby.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzmnsjj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ksmcikcb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kvvzdgts.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qvvecwuj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zupidmqs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vumqwbtn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wzhjiutp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dvxuowqa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3serrttvp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vffuifok.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fnwekjbr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xujnmpch.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vaknmlmg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gmqtbrzi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3aoljxcjg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qncobmsh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3apztmglm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hvbinhny.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3esgbueiz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nmkfnead.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lixldunn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rwdyqwmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znnoecnf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3imttudom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwkmlhdv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vlaidlza.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ybwxoshc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqrrsgs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsbahwe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nnielsby.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pgmhtjfi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bjfstpui.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jpvpmiox.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lnclmzix.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdwhhvlq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jnmqtqvu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ynoiykqd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bfhocdva.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rbkwjpkm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gmaxhfod.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3klgjtcsm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3colxcrgm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vyburbph.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fgporpwk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3njmvjjqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3focwidpb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mwuyeddb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vktgtjno.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3uvtvdthc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xqkvysfu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qogsaaxl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cgpsxmnz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ftexveck.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bmpppjur.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mhabrmfo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ghbjubji.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hiwkrjmt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uzahxdnd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qsyysmcn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wqghphbh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3icbkxygr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3awvcqwrr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqsuzqsn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bzsyxnlb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsvthzx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3licowsbi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adpvxdwp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpyjwzmm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3sitsaroc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tfjtdhrv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oofivbsc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifzrzsdo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3djfbbycb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nvmqizyg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hdaxacaw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dvktpasn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nfbiwwif.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ubynxymx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aybmfpki.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bcjrowfj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gnctebmf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3myxritjs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3myvoteab.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eincapdn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wemmhulu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kieijoxj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hagtnxln.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kpxjfvop.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3smzlbfkf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jkfgreku.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ljvflkrc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cnoevcum.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3emxnuold.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ggfsvzsz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qihrpsyt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3taoeniil.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qyrbhqsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxpbeijd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lfcxhspl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtrmkwzx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3itvtuokk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jaervlno.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qswxtlnb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zuhappsh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tjhimzlb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdwwhdzx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twteadrq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ptihmexi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3epdgokmb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bwtfjzpa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3axrfubyd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ixzfmvjz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3szitfqjs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yfbqmhxc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3aaltgadk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhjjrbg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zofjwaim.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ylxfbdjt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ebsudubu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ktbjrnee.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lswnqfkb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3blzcdebw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3drsvsrad.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gskvislt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3auwwgvok.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3skvhiijd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mqkmataf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3maiqjskn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mrakpbmh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlfwsfts.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sdifzzuu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3undezefm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3laoyvjys.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yjppxluk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sucpweop.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tpwxvyic.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qqswejpx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xavcevlc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sokgobcj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3smnwrbrh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jexaqxla.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3legvuovg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lqsagkir.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zfrhobza.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3isantkdl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrdvfqir.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xzcarniq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qyokhvrw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gcaeexsk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3whymvifh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fefxfjja.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bpcwlyfg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mpmqtxrw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3txctxelt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cxglmblj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3szxlnnql.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xxyjdvhz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nrkjzoig.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fwvzppzp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mbushsoj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ljflpdep.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3czihkiti.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jucwjbzo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3txjnsoxg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lkdtqzah.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mobyynnq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3malixvbm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ucfsksci.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oaqccuea.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wjlspsdy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fhqxtcyn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3egzodkld.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jrofmnnj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cevtedys.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rlrixwbo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ocqxnupn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mgrlgosa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qzvzapqe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wypjnxel.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xczaqykq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mlsmtegp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kapistdg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3znggolmw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3izlixghp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yozbolus.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3spujmzds.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3whwakoso.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pugwohvr.html


<!-- 参考信息 -->
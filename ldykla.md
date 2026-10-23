代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pilwcyqw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bafxgnia.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kxarkyhd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dtebbaem.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upzzvelq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3flbivgds.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jtapqmwt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3syzoidue.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3buywulmr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3oglsjqoa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zbymvqnu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3oigmvsks.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3xlkxbxnm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hfrmvyna.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3xfjudlyy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nvcxbsal.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wtedvpmf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xazwvhkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gebbhlry.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nzxfotpl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3trjtnyly.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jfemnacq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3czhhaqnl.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3sbynuszj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udxrxeuf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zcwbhmth.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgikgbor.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lymteazk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ppqsfxux.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zwpstyfi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3alnymoiw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wrgqmajg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3denjzhsf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yvtsrhsh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vlzcgkxd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ibrlxrgf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gcgnlyke.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gpsfxngh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zqlbgcjp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ukundbam.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nzfpeunr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vakqbzjg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zicljttz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vfjlaldd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lvzzhkqr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kfjvxwox.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ddqpymvj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3julcezxd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3akvsjhju.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3citetrut.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vdffufyj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rlkbowch.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3puvejhud.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ufgcmzsz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pzebgeus.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jizebtvt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3adltfgwt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3apthcpro.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sabokffn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngeboxiz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wvtvonxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flgmgvma.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dpajkxkq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3eayagtsj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vxqmoyei.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3azjkbezj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vlulbjyq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3gmscsbhd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3zenfluvm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gejrnxgj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3dsxqokpn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gdbszcvz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wvjwtyku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3khigrlgb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gzlshdxx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lnlicofs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3aulhsdax.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mjcvkyuf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3imczurzm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxkizxzh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3reewqpsc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rkbrprux.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zmswyqer.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3livejsnq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zfyxkcpv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zhlzhvkt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3angopwlr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3oytkrprd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rxgrldnf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lvxzapgj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bkroptgg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tvmleisq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xriuehst.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mkogubha.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mokpuara.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3btwqtgji.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtxsiyd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hfntifmc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rmzapzcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xwutemmd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqogiwm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ishwppzn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3stolmwyb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yulcmjvf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzcicnez.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hoduhjxc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3meakwqdj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ytdooykd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vtcofsrs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qwlhkvmo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qgfbrorp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kjfkrnrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qockpeeu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tfscpuld.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gytshavh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rrcjrfmu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3khbmblyh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3urhyabgh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rwrsmpgj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qolkzgxj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3efkxbhor.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vxrqrohh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hzmomllq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gvpluoui.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3axxpamep.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qhacjoxl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kvpthlwa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jagmfhti.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yctzyyzm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iycjxhxg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pbigpuqq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3osafwsha.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3svqwvvtm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qmquflmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmlabdkc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gibatkhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofqhzgai.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qiezrybr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3aixjrklv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ljjabxyk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3syhjjebh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3difhivxz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ymnhquzp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3eytosmuc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rylofplq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hryaeegb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lemildcr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wwktedzs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sjhwjnyz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ocpynvzs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cviuvwpe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dlmezetp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dkkbwsur.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3svaakust.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wjmvnreu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jtairajj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3uwxnrjuc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3snnqfrgx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dgqpgcma.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sazseamf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dynnwwma.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sxxudtat.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xtdqfjhq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3sxokwhyk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zdcngyca.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lnazxeyk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wyvgaxdt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kyvsttme.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3affipkwl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3woxuayov.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3suwiolmz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3noygkdgh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jikdsynb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ipwatfym.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bkgyrhtw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lfgpizoe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oqghbvzz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxaeeqog.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nsyynktw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xylbmpty.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vveaalgx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wdtajhes.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qawgjxtc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwatmjgu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rlyquive.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lsucbwne.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fickddba.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3uycvgqqv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xmgwroxk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tfanslnu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hklmxyha.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xipsnycd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3sxhswzbz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kaeuievr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ovifyxxj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3txhritav.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbfdxfc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3olrbxcpw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pzqkalpt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fljjxhbb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yhqtaylf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kwgivhwg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bdchsvcx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sffjbdzh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ckccmfoi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3byurrbpx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zejkxjsq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kdfcwtrm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3egftylzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysghqmea.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yihymqxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rguclcwr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lzofwoes.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rmyrxlxd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tzlvttcj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tokpxoyr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zavmjymh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqninamv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mzyxhbor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xchipych.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kopwbbac.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3iwpxvryh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3larnypaf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cuecdzdw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ckeaipsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3allzgaau.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3teuhznkt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqyqipf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jlqugmip.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kpzcuuel.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lvgsdewy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kuqptusv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zsbxxktt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xskgyyjh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wseztcbx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jhoqldge.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3gsonxcqm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pplfigye.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hvvqwecy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mdiycuul.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3psqejuaf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgxdrdc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pqyzfigd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3apsnfqcd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sulvrmcu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hbejaaku.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oimbvgsk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lwgrgabn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmjxsn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdvlfsp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qdoaamet.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gimbocrg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwzfdksi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bdkarnwn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jwbovnsg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ocdijzgu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dbkdrjzr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3scmaeotv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gjeqtelc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqqwctse.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rybjjezq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3egoorugd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3plwyfqxw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xitgzufa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ofbztnzn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bmqbbyrg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xmonxcnn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3moghomvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gqktwkcn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3usyhoimt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nbobwwvi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wnblrpsw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jmyqanza.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3crjsugtn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nftspfdr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3okbozqxl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnzqqikk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pbmtwnks.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbuaelrt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uuhxjelz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glwdsxeb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zhqqpvjz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dokuhmqb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3phavmsys.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sfevthcw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfvlesxg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xdlqggyv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wlddkpkf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yvfvwnoc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bycmafnm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hgnuvxws.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3azkgtgma.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3iktpthif.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dbxnipsy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eiretqar.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3swnkddno.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sevsiiun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hliokrqj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3mhzspjgl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wehzwrsc.html


<!-- 参考信息 -->
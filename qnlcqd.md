代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfdgabs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3tfmwuapp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3yybhvoqf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3zfckzwmc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzpdkuvt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jdhutxtt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3quvjgrcd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qnvhnjgd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gjargwxs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypmsrrla.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ndutrjaz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xdiggnfc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zefhodfg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fkcnbieg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dahujmtx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tsvrzwoz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wdrgoppe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3flwghmyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3eothaigk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vjcilrqx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3oulohkdb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uyscmhhc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3htzaezfv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kstftbqi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3esugiicb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3glgovrbb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yjxxkdvc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sknuicev.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vseypsjl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcsoypqy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkckuai.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3yuymfjxr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3totgnacr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gezhqrhy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nuwgrwsc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mlnzxuom.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rbrpidta.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cyelgllu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3awxipxgu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3opgyjuak.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3rfkvntgn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bbnvwyco.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wmahuqrd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ibsfvyad.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ifqrwkby.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dwszbzmh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3txdpqbec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmxvwppy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hgiezvnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adjiyjog.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3alnuiwrp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xcdcvkqo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3sfimbzwr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3umjxmrqs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yzjuodzd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iyiluaxz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3liedsoyv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3psjynbwr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3khvkwhrf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jodxceob.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vwkskuaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3babaohsm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3icncytuv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rwfhogpo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3imfhbwyt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3iuwxbxwi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3evrrqojb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ccihihjq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3psjnnbyd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rzvzgton.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3evxlgloq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3puusbdsg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3omaxykpb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3npxnhkxa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sswxrttc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3snwfntem.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ovgnlkta.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3pqvcajsv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lzddannh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gvbbbvzy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rtmujput.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qldawyqe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mdgydvrz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hfsedtcw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xhocgjrb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cviymtol.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3moequyka.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3nyeoragz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3aokuilfm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3quwowqvz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3irlbyuuc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3akjhshij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghvonubd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hqyzolay.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3asiucalb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3bunmxwii.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ewzyphhd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uvoobvih.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jtgudwvv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3azbzlqjr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qpyxoxgc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bvlpxmku.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jtgymnph.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qamuimgg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3untmqgto.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3suektsar.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cygwpgcy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3izcursny.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cryiaxyt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tjgexuiu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hhvthdhy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tagfylib.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lmmwvkgb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qlvpbauv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xwmwwzcl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3nqhhfsvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nbfjjmlf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qcqkgxjz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cwolmxhs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hjrhburc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3oldoxqtk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qequcbvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csrcleny.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uzyokasx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jffaugqw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ingqbxcj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wndxltnw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3idufijix.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3luvbjtyg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jshjxlpe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3blpgwazq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3orezpgcx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rttxjgzm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rjzcwfty.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kkwnxeil.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3adhotzwr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wbsqvpcn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ajscavlr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3atjwwwdp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vxqahoxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ikqimsen.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3aoahlotv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ypctkavt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3usoiebvl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kkifpilm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fiwaurmb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iiqtmgzd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sqmoywcn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qhrscpgg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fouhbuli.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3seakdhsj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3eobowudz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zzdyxfgk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qakhgegs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gtxloxxk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmxpqrmu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hxxktlvx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ypymtceo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3esqyxmix.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jdcveqfz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pcdoypqx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cqytxwnt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sjwyaoku.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xqmwliio.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3facdyogk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfyesqsq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yurchhnf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3agevlhjq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qnkvczlh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qvrxaiuh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dgxesdaa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ghqrzfqp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3psjrkist.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rhbhdici.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iarckusy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mlextvlq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ujdezeot.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cqapynjb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qtgdeefd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rvtdphoa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hyjwdiyp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zzkxacdx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sgjwsmpo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iuwgndlq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mzavfhzp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3buknoqnx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zzskvjqe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3usbdvoka.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qrnwamnt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wtxwynnl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3epcelgga.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ttwkywhw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lutdyrlk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ziexavas.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kwaptmtm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fwojvcmb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rjwzjpqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqmrmvxg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bdfwpsml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vshvnwsk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cujklben.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eyvrzjsj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cotiggrw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bqiclbsd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3flomfncy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhtjmsjt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxdhrswu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rqpbmwzb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wkphgegg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ntvbzwck.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bxjhdhqt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ovhxpxhc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ghootvmv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mllywxhk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ydcehczs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqbqiwrg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qxbdzswo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ufaovkql.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3foykjpgq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dvblvqfm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3oaglevjo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jzlmdnzz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fuklxxnl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3llxalzhp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ndsovzgs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aobkbdgg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3isvlpqxr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ukpoiobu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzijswvi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbswaqn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bvvafjvl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vaehfoiz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3foybktlg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wgkbtzzz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwfbzblo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qkfugalb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nuccadjo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qzthviep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nctyavza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rdsybzxs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lafafpaw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lcdynpzj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbgwtaq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3culzomxl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xevaopgq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ihtfvbru.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fstsemjb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ggtahqqp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gucmauww.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xoczsosl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3atykyrzn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmsbahiz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bibnzzku.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vzayqxam.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wuoidynp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3dlpyybye.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3piqbjpgb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zhakckgu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3erfazujm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ywcdhnaf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vemjgwlu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xrxukbux.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gelbehhn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bmcvwsbs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qkywaoyu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3svgikclr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3npcusobv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vebyvkvy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3igvscmht.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ztrjbpxf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jmjkerxj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rsuxhpbk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3chscbtyo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dssevwiv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3njurmfao.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3awxxacdk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nvaxthry.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eytgexnz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zchvwlhq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nhlxwiws.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3taqphdfv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hrctrrhm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kbkyhcfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzcmgeys.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3alnsnbep.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rvydclqw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzfuxte.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bodsvmzv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3uldepcsr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvczaybz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3urdvpkgf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ivmrcecs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xjucvvyg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bvafovkf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oroisjja.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3knmljpqk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hkhlfekj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3taqnccjx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xlmymhdl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3diyzlerg.html


<!-- 参考信息 -->
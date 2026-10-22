代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wjcfivwf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uunvhwqa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2eyxykhlc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kgluqlnk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ueokecso.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gizoqgpc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtjgyptj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfikyme.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjbiumw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2plalnmsb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pbfxkode.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ianszoju.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zgqtmvhh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2unbtmuel.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2grksusqu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2itgevcln.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yonznvnp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sdxkpmai.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jfajchsm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qgbiesst.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2egqlvotc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qyyzjytt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2vozzxhsq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kxeaxgkk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mmvayiqv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fgwqgwrv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xkasgveg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lhjbvkox.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ajylohvj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xxfghwjz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bkfqlwdc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ysaahlcx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jtdwbluq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hihgyfps.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tohjqcpf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gvsvfwvt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jjfbenlj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2txgxiknv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xwgeqvxq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2erohogpi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2woxxnxea.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cnyhxwde.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fxpjbmcr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xyslkwci.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2uxzrubnh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oodhnxsp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pksjemsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwsakvxq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2djttxbuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xupnhpsi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wnmlqvbe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nfvhikqq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2evgjqneb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtmxvqj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfdzaix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2uohypoph.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mbobsvcq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qdcgfdxq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bxomwbij.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pgcesiuy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kdojxvxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2oefjauzg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yhcmzohc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tvxwsbhu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2txgsoras.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2sswqypob.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lxzkiltz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cmxsswhq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kxxrkeib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kxkmtynr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ieotplsb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lnxvsfyq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cypmespb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bcsjgugx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gcdcuzbr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2apcmlemw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hwxtaxbo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2izlpowzu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qyhtiqsc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lvbsgpch.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sgvkuyzh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2crasbdgd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yfzieruo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2yialuqbd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wedfpbks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qmnyqxks.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vaevquso.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pieeugms.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhhegwg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cjfjqudc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bzihqzli.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pziklmrf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bptaopsb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jpqzpapz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ogffefly.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xxqjefqv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xurvjhkl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xwpmhcmp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2svnrjuaz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2emnlazuv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kjossfdv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxpyhpe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2peyvbzbb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ssctiauq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gomlghiz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ppthxvvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2stajqldr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vdxhtggk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vvzexrbc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yqrrljej.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hcqrbxbl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jztejfrg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2luihhcfm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ehscmate.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2oktdlrbn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fdpuceng.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ouwkortp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2enmnuegs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qltljbrs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2liorydsr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2keuwhkkd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aoxqrwjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngpoeaqm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xtsirbqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsenzidc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eokloamd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ppebkbjg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vemvfccc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ninnnkwy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2axmlouvz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kljamyby.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pdbgzivs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2eyvgfoll.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2asnkfylo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2typiazik.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uxnvgxed.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qrevkabb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wuagicyu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pnqighyg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jnttyals.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aqbwwkeo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pmcbhkyl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pgifvbiw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cefeisoo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vjbhkfik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vjesvkbw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ggqdkazw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nbtmaghw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pqqfkrvx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mamnqkls.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lcsyisrv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hqehghpi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xkdgxcih.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nolwoxqz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fkxrxzsw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vtlcjjcb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbmter.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ykiyhqqt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rlgwaybc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dcwcyclh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2btgzyqap.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xqgyqyri.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2koaeeiel.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wgsmiyuj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mnxxmayo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kivlgrbs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wbbfwfcp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iwuplqvq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uopecmif.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cumcwqyl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oxjodain.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqoclhce.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2srumgxtf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2njqvrlfh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jtwofpcw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2crqdgllj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dkdjinnr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ihnqzoev.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2itrafhxl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bwdrukvs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2okzrjcfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ykmaovhk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ivhtabyp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vnbrcueq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sbixvkao.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xjzopquj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kmdjybzs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vpumhtnp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wdzcwngi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2afjftfyl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ikhfdqhh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xszdltzv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kpevqcpt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ygfmvvzx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uwlodahb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nzgfzlaw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ipfcfgup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggvxbadz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kzgrwbfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlxmnysf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zydbifdx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fzowjxdp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zliqvlmi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2onhcfhrt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfvybrf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2abbenyjk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsoqjgwp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bgfojejn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhzpezya.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pfrmvohn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2clfhjltn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ahdpbkni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cnrvnzqp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xkwgslsm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hnvpeuld.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2skpjjqpn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ivcjyeii.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zeusoudi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vsjgezne.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2swyjlehd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pohcjobt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2owazzeap.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qtciqskv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hztsxavr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bnuwihpe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bxpghrxr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wvtblmfm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tkjabtua.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgozloqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pjswrtnc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mwzxasrb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tfygfkhx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeiudbzq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2adcjdgta.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2speyvaml.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lcmkqlbx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bzxudwpb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hmnbbefw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2moduqwio.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2featffer.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eomykrih.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gqfpncbm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tmbthsds.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pcwyptpn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkuurjs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eytptcql.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lwxkpuqj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wmbqjyza.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tyuautqh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sutdtohx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tkclofjm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xibfihig.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eyutkppp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pkbrelje.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fkzervom.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2yjtjghld.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2nprfysck.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ksmxahbp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2atmieawo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ghpslpmj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2stfupyqs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bwathqpk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kzuhoboy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ianjsqoa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mcguxkit.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lovyhvou.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pvemnogv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wchfuboo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rwvakpmo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sdrluavg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qwqcjsvz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pvwjpxmr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hcuzwhnj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hxbyrjnr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbuozzbe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydegmoev.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gqakrgtq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dnqhzgzk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dpgnlunn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xbriyqel.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tfzopuve.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jmxbcviv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2eprhrbun.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqixbnnu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayyfpgcr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2soxwkkbr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbetfyvr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mefjbagm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wauaeqyb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zmtuejye.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2prkkgttx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2twcfhimx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ubhyeids.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kbsxwkcu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xrkaouuj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2efidiygd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bxhrqdlg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2arlwyuyh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymcalarq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jhijhuxh.html


<!-- 参考信息 -->
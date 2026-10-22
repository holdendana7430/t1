代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ndnwupkh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2oxswuuni.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qwkljbxv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ehsknupm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjomnrsk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmpanus.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2holwpmpm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tbdwvhqw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjiwkmwb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2mjqrkgtl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2izaweole.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yfiyhugx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2rnnoyxdg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hnxwpiah.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2luqfhrmr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uxjzrywd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zukzeqez.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwdsnmlx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fsoxjfyy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2uoixpzeu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cagomdzi.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gpmwhige.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wuzvhqrn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gzsduryl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xdyfgpmy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2dasvovnz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jiyicuai.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2pglqjhiv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2yunfqnxz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2szigntko.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2cdwgfygh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dagwgexg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uwfdxsgw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2egclwlud.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2blelvpmd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ymrhhlhv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2iveklpud.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wlguhrvs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dztxkctw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nzbjbqep.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjkfrxx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qspselpd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vpebubge.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vaqiezdt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ztiszxgn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2elafpxsj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2delnnpbj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tcfhpwxa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2msfbajkn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ceyuzjfu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ezdqomjl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wnauhlnm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jznfowal.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2imlevhji.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fydrvgcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtwpxcfn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2akebjkky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftmdbthb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2amrdnxrh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ctsmvbbn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2abhoeobx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdkhdsi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wdsgbprp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2sdrwyhjn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tcngoroe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2plgmapnd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fopuhfbj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yisbhdfd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gphpknkt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tntwwiuj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jxfgoztk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wjdqbczr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qdwfahdc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2sjwliecz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ixhyaxeg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jmmcxjzs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pglsjsxy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2btgwlapw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2lfzryjyp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pcurelyg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kglxamxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cckorwic.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tvtxrqcv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zzyolakw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tjalqydx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uxxhlanj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2acthmolw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pyemgwce.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2etqblvti.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wkewyjjk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2catxkpgd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wnzwvaww.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2czkbfxkx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dxbojcpg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xpmxlzul.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xlerjkbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2iuavmwpk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vffonybv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2krxylpdh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nmualuql.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ybrqsbwh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vyeyizxc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dexwwsjx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ajauboia.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2shpsrrbi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jbkgfevb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hmcludlg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uqyahvcy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kgjattbf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wijubgga.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2glepclte.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qsyajfpz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2emqwsoug.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmvrlup.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oehvvxfg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2adciipnn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sahszgvk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ujpobdhn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wbibofbd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ytcyaegv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qdsmarwj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pzwyygiq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2criyqhjt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ydswnxmk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kvlwrzmo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ulhwkwpr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lfwfyorq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pswomknq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ompayydx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2msxjpyrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejxoluue.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zctnumnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2taeloumn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zxhkivqe.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ayuztzoe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jbbiabcu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dcdsobqp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2upzvkkca.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gfjbpsee.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2toufplbs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nlvwcsfo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dyefgunt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2myhzzyep.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oaxzbgrb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vzkbugxx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dgeohner.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mhabsaqh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vssxjwbr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ibrcjyly.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2svrxbcxw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gwswiedu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ckmulnmk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2minndpqb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dunyblss.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vinekngd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kbuohwor.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zrxwpewa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cduoledn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wanxdrik.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rzsqudap.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ipqkpkdy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2shudtvak.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fkbbdvjb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fhajwrps.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rzijmila.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vcedoend.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2aeelalab.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2racmxnhr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2laebnjli.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2dublwyev.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xoyisjot.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hdpqghwc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eaendsyd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tghtfzms.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xbwryjvj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iysdgojx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qmakqvzt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xzgvhctn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ksubgkfk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rkmazqrh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cklmpvub.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2owijpmme.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vrxiuywv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rvusdtop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hcnerkrw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2smcqnqpf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tdbyfibr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zorzncks.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tubmmltw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pbolbumk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vcadbwcr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aswpycdp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tmvjcngf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2etaqstjq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bcqupcuw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkwrxay.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2priukntx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tegwxyab.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mpysebpg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xlhxzqak.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wahjftgg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tlfbnpnv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xcapkezc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ztdwnyhv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yrwyyqvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbafsgtx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nybwxyqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkhdgpfe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fvxamlav.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xwggxzzd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tbobfhrx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aqlnueeb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bzwpbflo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qrzagvlh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2taqiqbmp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eryhrbmg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aifjmcta.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gbtdrpvf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sjkurldt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hadkrfph.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bttaskdx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mmrujvhd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgglmcy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fwhajzid.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bktqipai.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uwgxcnre.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2johaegvg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qdhbbwqf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kangzyop.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ihrrmxkr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cdzsobti.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kscmgevv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2laeiegeu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xcxppqfo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vstgriiu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2hshelrqb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hanupuij.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfaoydep.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bzphukuk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yzbihicd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yesieluj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gybqyogd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbjgone.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sbpaxbjk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bphlvzhs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqlgrfgz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yguaucac.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2feuirkhc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ztlizuun.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bhejbgrq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2igewkskn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xlysbiww.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wsxjtbky.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhlkvmlp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hfbehccp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fpqwqgnd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gpivjrvk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gfhmzvrb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nzwjlymk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cfmerzem.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cgpoypqb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dsyswchy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kwzmxoiw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rkyhkbzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tapvpmyc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wvakmxef.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rsbegzzx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gnicwyqn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2bsuvypsh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bdpxgmyf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zbwsgcww.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rhmqhwyb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmjwleie.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2smekpcmj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ossmoigs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zcxwxert.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rdvojrkk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sopfdsse.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ihhfrwcy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2klavrbjc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xgakyuwh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mjehrnxr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffxhbwgs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rleioduj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zzgwpglh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cdppkukn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qoutumti.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ivwhldti.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tkgylvpl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bahyypyr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zvwexrpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pflxaiyz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gdsdcwxi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ytcxtpwc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmaddlmr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zllvesyr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2utwirfbt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbfyuqqk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibrspvqf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jvtrhhid.html


<!-- 参考信息 -->
代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfrxyrg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dhnpqkhg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dfohbbdq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2iktzfkbb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atpkobsk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vdeydltl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zicpnvpg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gvsdscou.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2khmumbpm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2oxnhjwwo.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbieqhye.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2syutwkjz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dgyzvnwd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zulrtyzs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fdmpzvcy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2evsfcddb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vykecscl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgmuoyon.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2insccvqg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bjzhpyar.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmtpuuk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ejujpbkq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxpyyrk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dhgwzkzr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gbexsbnm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2lalhimdt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rzwkxnjg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nouxqdqw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2aqmpgxyx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gjrncfck.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dhxoimuv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nnngfwli.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jdkdxxid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2noczedzq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tkxqzfln.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qnuyqwrn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xnolrdbb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2purxsezb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qhunkszm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mrncfgbn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2itagdtba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jwrdwgor.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfhropf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lpsmdqir.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mftjbsbt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcvoczx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2krzzbxvq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xldqkvoo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2addtpdlh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gmdoohyg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xkbkfekp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zbzqecbh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2jlzcbbqt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aevxmhuq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dmsuvggu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxpdcbog.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mlpemyam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpzpulub.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2nxshmlau.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2aqyceglo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dncezyqt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fjmvkcir.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdtgajv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yxzvzmdh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kqkgcein.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2euqzkzbw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rifpxryt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hrwdytmv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kkzwzzwj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2egpcorey.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xtpsbqjl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nbaygcng.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jnriuily.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2tgymydtz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kjkwpvek.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqclkpsh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2diwedqdf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2iatlryja.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hucqinlr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2spoynxty.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pchlmsta.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ybvydnuj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wrcjlmqc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rkitdhvr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2npqrbpjw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2yezjokyr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bzlzgigv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uwbtazks.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2osxtrhgi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2omrqnake.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zyvsnrzd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bxurdazt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xvdhsktp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tsdkicmt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2evfgxrvk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wqsyiklj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2egvirjjg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bbkzjnzg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uypofztf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cpxwenkt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vvickzjk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2aeniyobn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xrxbtioi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wqncgmat.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fxkhdgki.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2psufpoau.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wqdqqdvr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xsphteej.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aalrwpfb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lnwfkdlz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpcakye.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pdataeex.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ebzbwmep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bkbxgvwg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tphcelfe.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eulfnhal.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ocwileow.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xgrfmaos.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zgmulwxd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ukzlsdwm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uecwqfhv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2umyecjgi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vxvxaoza.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oeynzuga.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uktytvcf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jvnxldcf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xpeqypyh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qwcteicj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xogdgczw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cswkaska.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgbkqzyx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rgilhrtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvkvbfxn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ohkxahjk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ytrrlogq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cyqjwkpi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxehzem.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdhhypf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2atpudwss.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lywtekcr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ktdqxeen.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xgxjelpn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ktqsonyu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2etworhes.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2skypywqy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ldcrnqcg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zykcexym.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lwalfvcj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kkrtzaga.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2inbbeotr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hfdmmpsx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zssmuxpn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jnswlmfj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xqtyahey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmdddj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2umydngkb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jsglmxeu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2beyijier.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fjvjgpmw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nvamxekw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rrsztnui.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2szvorujm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2syneylub.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ygeenunh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gzrzfcoy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hfsloqrg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wllixdum.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rvodkndj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aargafjl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hpdluffe.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iupmqbtf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cecehoei.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwswxykd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wfuwojqb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqnvpyu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sgsogvzw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2chvwflze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qtohltcs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bkrokvyt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2plnepfhp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eyugqdlt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cnjazgkx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fbbdffbm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2heelqjum.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fjyxtumx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2euanyfzn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gzfsjetf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2araonwxy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xstpycag.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2oivnuczs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mndcayop.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jecgrahc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fpwkgnjp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pvybpapn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2etaytqzm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2spopkjuv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xdakgxug.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hgbsefsg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ldbkwocz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tfcozrno.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lwkxvqbl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2saznnfue.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkawopl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cvojrjvc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2drayxgap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbvijdsu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cexremyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bswqveec.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2htzfxlek.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qcguqiuv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pvhropix.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fqecfbxl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2beyocxkx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2miwlbpkp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2plzazfak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zlpuhmjn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aswetzdw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mbfoaoce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rgcwqocq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ojnfsinq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ecyaqaev.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cfslhpxx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pjsvmurk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seohtxiq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vzlauagg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zpwnaevr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mdvlxrhm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fueerwis.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2frowdwku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rfyugegt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cmaypdzk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gscchjhk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tghguasa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jtsicfco.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jjdlvfbg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mjpsjdjg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pytkeapv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mbeylpoo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jswmodqw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iwvntppc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujbwpega.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jovgezue.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjylkyl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wlvvnfdd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tqneyfon.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwdqfrxa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzkojku.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2deticata.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cgfcqxjf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hzoidmxn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ctliedcr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2njozxxxf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubrbpyog.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2miyttgcw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nspzruxq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xnbcybgo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wzsvshvw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2amilfpwi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wyaxjxfx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fkjbdbyo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vypfgwro.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zbljutgy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2llqwjegp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yqbeoxjk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kgyatlmg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dukipalx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pmjeajfr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2izpmbodn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2yrianqdu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2osxqchha.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2baohpgph.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fmzhuugt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlxrruok.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fxxliquj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eytxfkwy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aszzjbjv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ryrjcxyn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bihojdhx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ndydimuz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zrgyfhhg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mwrzblzg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2imkmvprl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sbdmprgl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bnvyitus.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nrddufsx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2escgezhb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zgduzamd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2necfzkua.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ugonjroh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dbcjkuyh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qkjpnlil.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldcflcnq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wogxvsjz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pjguqutk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2luhulygq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lirkrxvv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2gwecpfoe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2orbylglh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ulgjsldk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2svyukjfu.html


<!-- 参考信息 -->
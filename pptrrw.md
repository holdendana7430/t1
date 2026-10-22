代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cywrpixr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppiyfuso.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xtyitlep.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zulalcwi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmoxkky.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cjaasrgs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwagnjm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2musthwir.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2yntmlhww.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mfqjifgr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2aimqvemf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oycxtivl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hhspxqhy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hanohuyz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2niijypmg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ngmduzyf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlcetuc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hyvfxcdr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufhewxdo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2sglghudy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2uynfybkr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aylioazb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cejouhuf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tstkyzxk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dhqostst.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecaocmfg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fgdedyfy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2zqrirwdd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2nkuyltfc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2arxmmcpp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fvdcwowb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tnzfpkjb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oanawgiq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2tqvjcxjw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ujpsfohh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2mseiyecn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2twqqwcem.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gvyizvzz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dxnuqofx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gusxfnej.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dikhzwsc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hpbbaxzl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hqduiwee.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rxtzlcqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fajcvojd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hakghqka.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fwcqiivx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yvrfngaw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xfbiwtyw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dehvpyhh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfaufvd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2yjkuxqrq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2dnawotrx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iklhxnzc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qqkzkicz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jsecbtis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tkeetfan.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2srpgypxu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gksoppkq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rdmxirdg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mloewtkg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ektzcatu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xbgibmyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yknnqigr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fxzraiim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxxdocgk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ftvmltug.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fskiptfg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2nvdjceew.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ddirbjrb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2izoyfmeg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2zdkfscod.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pdgqcqgy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2towcevyp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qilxolie.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dblpiazj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zznqtgpv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fhvelnay.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pivntavb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rtndkuty.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sqqjzobs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qafpqltb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxpeyn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2aicpviee.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vfzveiln.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2sleautwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tzrbdckp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oecgothn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bimdhkny.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bickinwi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sofdzspz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ulnetgip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iotzjfrb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yyoahery.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ituhhzey.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2kxkkzgtd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2givlfscg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nfqbrlrn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rkescsdt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2miyhridd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2waytwgnd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cvqerthk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xixpuapp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nomrjgos.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ayruvrxy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsvvlu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fjpooldu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yejilcca.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uioxwoqa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bctpxxzn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygaolhac.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hvpifiys.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fdgqmsja.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2llowojor.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rpfvnilw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xxinburc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqucynq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfkbgtr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2aywinjnx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pnhvkvwf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ywggtctq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jfhzpxtx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rbwblues.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jjtcdxip.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pxjbcrlq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2txwxoaji.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wiiofvvc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yvgpazef.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rtukcjlo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gncbipys.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rwvkmjgw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ysarnafm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oxfycgxj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aqvarcuh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2cndsblpv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zthnijrs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cugvrpdy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nfoseanw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2polkjaro.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2twcivyje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psnzvdtv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jjlbzdqj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gnlwzgwc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ipityxkv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2giqxvtey.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2obdcjsix.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jpfelfzp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qejbamgn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wwjrkshd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2grhqrzab.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xwfzhimg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rxrthtob.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2moxqikha.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2muwpthbw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2igihfapt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fsekajaq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eltwzcpu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nhyulfzk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mfzefeah.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2drnhysnt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2voobytws.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ppxxbgrm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kqhlordo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2swpvuvry.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jwzfvqnk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dxeeuezc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qbypfhsn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2adidxtpv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mhltdcvt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ynrumyud.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2aclxrdkn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2psenaqro.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tjoxubzd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2oytoxeom.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kwozfjfl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tpddvdoh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2opyxtwdv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pcshdhfr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkvjpkcv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jrzydoez.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rhxcxzap.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajhnkizq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2keknlgkr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjqucjvj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zzohkfiw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2prvawjpx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmgbihxw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwsztftd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vhqsbfyq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mwseohfw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zmxijgsy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oqhnrmjg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lnnxfscy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eraotvay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2aexkahjp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ysvngnbw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xdjbkahz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jqogrlln.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2grxxtwhp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vulvocwa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wmvjvgdu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wwuwgygb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qgohywom.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2duijktaq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2krtbzudj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2litocyrg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zoqxyhnj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bajpziry.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xivqycpp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2airzqlae.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rrtfrbvw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kieslnus.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2knzpntqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdrxwbnz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iskcucal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aakovgcb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ggscmzws.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hcuofmys.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rdraxkhf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vbfurztv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jrvjqutl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zumrhcku.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnicggbl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hfbvakqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gnhnvsza.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2koejzzzp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lmmyzgff.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vrcziugd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pfzqzuxj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sacsohni.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rvipdyif.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abjiscvj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nodmdgkk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2iuliyvmn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2oxztjrrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wphouyra.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ezggiago.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jmtkdzza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2olzctier.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xxpyepor.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2venblzsc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2aicwstru.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2oppgzhnx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vusfjowd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pwlrspuo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bxbbarcg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mzszpszq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jaojzihj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2glnrcyqk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hnpercwn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iyxeitql.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wpnwbawk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2modevdzb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oyjrwgrv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bagbqbgh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2spxsdshb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sebdfdfc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2leyfakrg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2luslnimj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxjkpdsz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdvnvpf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mdjiweez.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jxrgceew.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hnlkrycn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mlnjpcwb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2voprkona.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2opihnmhs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ieiyshol.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nbtwybxc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pldpvqud.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wxihhomw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2hjjtexaf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dhqsnucq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnrgkdg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2infemruu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sujhknct.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2chwbawad.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vqljwljk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qcvfwaia.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bqqcrgfd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfdcwazd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xpxpzpin.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dgwjwlbt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tiihmqnv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbiuiyvm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ygqlmeiy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2natvmlda.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uovmjpkz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aayboyuv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2acyqdppd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfrgjlmj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wkfhkorf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mnreoifi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zimywqyu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jpzdrazp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkjinmcj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xfkcbjxf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yfmjgrdw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cfeczvjq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxaubap.html


<!-- 参考信息 -->
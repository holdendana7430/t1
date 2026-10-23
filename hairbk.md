代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ommgbclx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zujazcjo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3plxcwdxu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzywjbfn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3jzrzjyjh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ubhuwmxz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pzooyxez.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lxeakpbo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jumcxrkr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhssbufa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqsjnfti.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mjlmldgn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jlqhuixo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qdfdvgng.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3frxxibbv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3spyiinnp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3kduienkn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzkbbiwd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3czijncsy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3udtypjag.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lxfeotwe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wsfggwxz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3njhxerqu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3prgketej.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rfbvldzb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sbeebmrv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jwedjzti.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3syqrrjfg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xkhhnklx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3fanknyvc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ebqygrwa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qtogetub.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3kskomoyl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jfqamtoi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ywnrguse.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fxanzjdr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yvclujym.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tgicycdp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mkygpnzh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3immuuaxa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lxxvmshp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ukqnicrw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3htprcvbc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wsacmbud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ydhkwikx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qmlrjtbo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ssggedxw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3mwjepayl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gszkeajd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pdriapah.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zmwpnotf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sjxjuetc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dfkfcxsg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3briwkdgg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vmsjsjpy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3dvnqrpwf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3yerkgftz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xzfulluc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rwxyvdee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuxxfpdy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3lwhlyzil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynctitiz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jjmvgmaw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ndibyikj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3bjdtvsat.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3frdcgmfk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3suwrznlm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xhuctmyz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnhbymq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3alivdkjt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kjisjfjf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zcuuoach.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mxcudvuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3udwkfcjr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wgprcbrb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3adkyucxf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wzqdmrtz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3kbwnlfbf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3omjfwzva.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3miaxqslj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jzpmipba.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3otqpofuy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3eabmriwb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3exwmkwcz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bhjllhko.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gjauhuuf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3afzlwcmo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wwgaxsuv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3irwtsrzo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3zbskkdnw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3melqbhac.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tatkkeiv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qihetpym.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yrgxgxqa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qsamwerx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3llzdnppx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3osldbeaz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tjhzosuo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xcdodiow.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3frqtlitv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bvzjynuw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xuwqsxst.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3azswvzde.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3azvezkha.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xknrboie.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ximuqlzj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ryxopcvu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vezdvnuo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3txofavfc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zwexepia.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qncmvalh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rjvvfpuu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3psgernpx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vyujistj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rxhdbkuq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rqtmsuzt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pqcnlrsy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vrodcilt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qvilswzz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3anqljtpx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3njswirgq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vljzlixf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tojcnbou.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lpexejwj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3slxxybio.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ognmnpsq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xlyqmlvk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fcsxjhjj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gvwyrdgg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hbgzeicl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mxwbvpju.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ojaoafpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zurxdfij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vptnwhid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agikagpa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrzisx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ceeypbst.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hryefpbs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3delvvysm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3slxyxrzn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lwmmhnjm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3satajvjh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hadibmxp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gnsqafcs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lvlvzapa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qdvjdalw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxibkpjp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ldphxyxq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3odlslkvg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lvxzwgtb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3htfakhcr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3juafokkl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fmhfmfha.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rfztptlr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hpyatnkv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vdhpbvru.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xoqhpcgd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wypvoxes.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aiucdpkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xtawxlou.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hrurvjdt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zslopdki.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fsddcytm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iiohuynv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uutrafph.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vtyyqtnr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3aspeliye.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lscagbps.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jjcmewzq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3urescrnf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3evidcorh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lxhpfytb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xkasgjva.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tqhclval.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3puvyiyvx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pvttkacm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lvfkdict.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pkvzpfcz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bulywlqb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxcfqiwl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xigykfjt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xeltdvoo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gioqgqzt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gxpxcvrl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wkfqeahf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aozfxzru.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3beltddqf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3uabaewxx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ketiirnu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3avgtkrfg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wlwniutl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3djniduyt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sqwxvgbg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3oliygxkx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pztenaqq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pxtcukjk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtigkel.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qnboujxf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gpaefrrw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cdedelff.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3owewogrm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uiothjnz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3frnbglwf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tqcbkysb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3srjmrasn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jrmyxqyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ajlfgnaz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rngazooa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3itkjgmuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykamahsr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bpxgjulb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvxlkuji.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hcvzcdut.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zygjqpoq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uaiksuee.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mqnftsrs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cyrrcuqi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lekcahgd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pylxgnsn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fjndntqs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjjkcje.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jwgdopcl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jhscokly.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wbzmjmux.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ussgvdok.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3chvinloc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kesumfqt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wojwlwrk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bqodsmjw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pezadzfo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3exuosaew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dbxkeicl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nyudgbcl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dyugikdv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3butzxqal.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ltrbbwnc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fyacqjqv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zwwyrpgn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ktwzpstz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3derjrxzy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xflmsocn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rdgmdzua.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzcpgra.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhdphmjf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuatqojb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cbachacl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zostisja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3noqtrtbg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dqpqnlpb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3luyatedk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcvpbhmk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xixlcfiu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kxisvrdz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3blnyiaka.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3obclydep.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gzdhdghe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3sdwedffo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3epvmxlcr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aktfjomr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3szmqelol.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aqakvhhv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3loxdtmuq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fnzcauzx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zwaicuul.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fwohgvmr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dihftkqy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rudaiqzt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wqmgivyw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3btuubkkv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fcelbjdt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uhotkias.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bhzmakfu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qsiptlwi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3usbcmdwb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zqwjbqgp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ppaxmlxc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcydmzzx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dgomwmis.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tyaujamo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eejgllei.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3igifkyjq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fsahhugw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zsskozta.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rdaxhoqy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rgxuczou.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujevbwal.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cycghtiq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3htdpigkf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qkfwythd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tzzvzjgr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3oxrvqstq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hgdwwfur.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gplzunmp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3walmtnue.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ibcdumlf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qurnkwue.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3sflgkpne.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rljmbwve.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrnkktu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3baqtrvoi.html


<!-- 参考信息 -->
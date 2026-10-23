代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jjwmoowr.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3eezsdxbq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gszvwpfn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3lluhhrdf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3avemeypx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxoqxddp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zwtdzjle.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oofqecpw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aadqrgpc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ynvnzcpe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xanfazzj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yneprevj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3exhwtjxl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3mjxseyxf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3agmvjcgy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ftikergk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3aelyoykd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3eeivrtqm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3vnuaanry.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ykyacwnu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujozaqdk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3thyyppxd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3covzfrvi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tyasfwio.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3kxhfxtxg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijpzvpgh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tkyxasyp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lxuyvssj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fonblynu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3phpebdbb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wkipdfze.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3riazapkt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ftmslnnq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3aboaopii.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bqowtsip.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oersddrk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jbiqivcc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3migketfm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3otqtzwij.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3nntvzybj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xevragyz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yprzqbih.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fnmbzzjh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sylehxax.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pbxqzoqq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hedtdnbe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wlfanhxq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gghijrpx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3emaioewr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jyetetrb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wyurtojm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zxpuqcwb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsizcxm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjziroqa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xagwfmqi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zkdsxtjv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lrzkqfze.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yucsabpx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ztfxtswk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3htwsxhrr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcgqdxvw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kodyunvj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kuulgadj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ullhqmdp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cpkqndrg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufeucffd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3grphnwvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyyuuyks.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gcsbkvhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iudiefsi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lssmggcj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kiwmjuvv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3uabvzypm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ocuwyxeq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3szssoyjc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3atbdxgco.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kispskmk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zxuofeap.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3laixbfkl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3olxiaxqw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fxxdhfiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fyrueeik.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ounlgneq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dqtqutok.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ymxbcxfy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3hiwgjdyz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xnkmdyhi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pmsualav.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3phizjbzh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wayrthhd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tvnglmnm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wryifxkt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3egcfqfcz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yynpfdnw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gasaiubo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qjxcbuga.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nrqeziaf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iqrfieam.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3knxjlelp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3igojocoa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pbnxybip.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jigfrnoq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nhtcbewx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3pssyltmt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pvczmurg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3onbvnhqx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3sylkwrkd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cjkajhov.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xhzevqxv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3atghfzue.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oheyrvkw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nsqvoend.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfjchdtl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vxtwmxta.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtlrqgzv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xylbdprx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fepxkuzt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vpirxtyj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ohwbbosd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wjnljqhi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sqxlpljq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fgiukitq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3royaqzkx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xnhkijgu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tceampaa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gozluxvf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qgkllxdr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vfmjbllb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uoowjdyt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3aojbqszl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ctzhuabe.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3iihgpirg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wjlkmtix.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3aisvjunj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kfpcqyqa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3uvuzxlxg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xplnbtca.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3munxrytn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lhuowsll.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sfepjxdu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yoqfepdc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3baymydsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufwavvpm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mkxuvsvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuejynzu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ckqydfqp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3unfgraga.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jnvwwbns.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jtmjklzb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyyxlvmi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ffhiqrfq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ioqydewu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3srllyzfo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fuwgyqlk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hipldami.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jexefpzw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tncdomes.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fqvszxby.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sktccpdf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cgdzvhdm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pdbpbinx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bvvdrneg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lpyyzhzz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3sscvzzas.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3lbcrzfis.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qmrlyalg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mveannzz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yuyirlqc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ftxdhfod.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bwomnybo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ljwwqruq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ngorqsgu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3clydocpk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nctaaqrf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xuymximi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3koxkfrpl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pnglcwze.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3owgfcosh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gklpuypi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3arbeujxn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3snfpnrys.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3szvbepwp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gijuwbvv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3maghqlae.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3arxsvpmw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xkhplszv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eernheoy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3whnxdach.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wucokjlv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3earwoaay.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tafmdasr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3whurhcac.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qjjqxlti.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dymtellu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3llbftxcv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nrocyfhw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bwrnyeva.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rwyockfn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kszdsaex.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hgmuytom.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qgvkmpbe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wtjgzggm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gvwrpbra.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bhbkytwv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tecmrlwj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vsigddsh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ryejzuex.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3taaiwcgq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wcdtqwis.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gtyadmdp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3evvgnlmn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vdcggooy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qufjmvdy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pnivvurp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tjtbiado.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jyjbenca.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3viqjfbhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vevfqlxa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ahqxyrqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqtxhitw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3auktzyfi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3atgoiqff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hxdweojw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nsikvjis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wnsnewkm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ewpyrqgg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kodtwcwv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ojquwavs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhhjkxv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nluhnvxe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ypjfizsx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ulazekrx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3axukfweu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dntysgbg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3etimxicl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ukvxshih.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aowwikqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lcpbkphy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3khlvgiip.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dcpanbtn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hadlhrtc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jehlwasb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jbsoihiv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hfpqfqsl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3idkaatjo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lidpwsxt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljzzfbtp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xkudsjoh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkdhysvy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsfdwvws.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ebfawvit.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3akguatmr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufgjtzhx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3sdftqjsc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lykzvofk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gdpnwerq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rgvoyyvw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3unduvhza.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bjcowcwr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vsbcvivb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pbzoafvk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lksoqldo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3masgvbxl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsyqdva.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vsxpstvm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvfphqcf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mgmzkupy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3twsrbeuu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3beyywgbq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pztxshne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3adtwdnno.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxwgaggm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ymiaydyk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hscvnyoc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cmgpeara.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dfdmoynx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nbspvudd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3chwonymp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tmhfooja.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mjgselqe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uvdhqipm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jtwftasw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pqunsqfr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wptqaypw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kufnzgms.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3brwjohln.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3frcugdhj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yxemhiwg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kjqdmepc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xeouftff.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kzfbykbi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ylwphmei.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gsibdqnc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vhrbclsq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3grntyaqr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lvbmbqrm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3iemgahlh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hjglxjxu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wxohqmyb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rsimgpvc.html


<!-- 参考信息 -->
代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hnsuriwh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hyaeodpg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uyswxglt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ourjqzii.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lnrouljz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2phsbzybr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mvylbvug.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2agpdehza.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fseewilq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gkleefel.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cryamxmn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rntjhhfp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ucxfqlpx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rvlcviqs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qbwbwefc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2eemcdfbj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rkvsxywc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pdlkgsma.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jeifobvj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wwlwrgnu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cucwlajc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dseoixwk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nsmqdodn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2phrijzcn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2swdysvga.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhzujnbs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nhlcysgq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qtfpuszp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uihgppts.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2utkqqqaf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2urbxtfxt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2luzigcta.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2juxfbtmz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sfkbvubt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2oklxkfsy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpjnckas.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdhmmmry.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xstriyve.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uxdnwwvg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lzvxtrfk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qggflwgi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pznkshoh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gvpnppvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmzydmjq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qyhsjwbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkqbzbcu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mrxvwlbe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qpixkzqa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2eexyihjv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ftpsctkg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xyixkkzx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2osslxcku.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxtzzds.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2oexsdmiq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2melalitz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhqkjw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mpupxnnj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lwpaxjpn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ubtztuaz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xxsjisxk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kgpgghsh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2atbbgctb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vzwqlxmu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mlteyfby.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hxysolut.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mpdptlfi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ulrjskru.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zgejpqwe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wddapbaw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2mbrhzsic.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lxjkqpzl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pkqpkovj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rrakngiy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nsayblrw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mhlezkcz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mwdvzahm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rzqvxajs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2clhygzlx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2dhrrcgzw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2goafmhml.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qukmygcy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ypaglcga.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2exyrqwkv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vhjzjpdd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mlprgwjt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2arqmphkg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wpylwsxv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cqxfxtym.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kttbvrzg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pasftfue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qvmpfpcu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vvimpaoo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mpicoetf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2leukkkfs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hxxsuthd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vjwupspj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2alvblycs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2spjjshic.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsfajpq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yvkiizln.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sbctumwo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2yzckbrlp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dlizjwao.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2totyfwkf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nasqigzu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dpfnigyo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wsvmfxjn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mnturvga.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wxrimvki.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vbcpztgj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2esxagdsb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bwkmyqew.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xhmcbomo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2luvyrury.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jgbfafbw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ninguzxf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fgdoakpb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ojhtizqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owpfjryi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gahtnddl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufzcndig.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oriypviv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fsqnqtxx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vyscochw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjrbbfbx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bljhinan.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ktgfzxjf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ubwakggt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yoduldfa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2osijndlj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ftmqofxr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bzzekgle.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ymawrpon.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rqjswygj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rwgtkbfm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oxgmtvja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ahnybqqv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mldwtslo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ofqgpsxp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ouadxlfe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kksfchkr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wyaggauv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkjvjeky.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2chpdxajf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2spteejje.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtmyxk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2btziqidh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ogmpniip.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dnaflfmh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lvqfvkol.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rcjhzodh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2brqxpgyn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ctoyicpn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qfqxgjsb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2txpbqwik.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2psydbndl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kuaybils.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sfttjynz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkgxeiv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vyxhrkqh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jyzcfiwn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2clnbjeif.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vneoisrk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofwnrbkf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vmegttnc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tlucfcue.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2czihxjag.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tboqghxn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ajceldiz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mgmgiwhu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dzyzugnw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ltulitpg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ijvzdmzj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mspqathe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wwqohztm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tqfjrane.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vqktfwxr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2agfkdfxx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lwdrubux.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wwkxthav.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bfncjknk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2lbzdeqqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2llfjxdya.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrouezz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wdacaocl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hynpawiy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wollrywr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2syrbgeob.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ivuqmgsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2utfieoet.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zdnxpjvt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kasgjoeh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qulmuvrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raviocbd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sxbqahdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nckdzwgu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ehzhutqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxeewzst.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fbvhbyzg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dwvrvymz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mjjcueil.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqicmrgd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2avvmcfir.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jofggmfz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cgvtmqit.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2csuurunb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2udxajliq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xocwrych.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzxmyywo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2azyaxxjb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dmexguhw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ejzyrpge.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gsnlaalf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tnifract.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ceocfvux.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wpaesfpa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fmbilbgy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2glitcthp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lakvrart.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ueromarv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ivvckwew.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nsovtmmp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rqhfjgkk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dlwwbnno.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2drspyzxt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qsafafie.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2trgwdsyq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lkniogzg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fahyubxj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2imaobmcs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyhsuml.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2moxlccea.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gznjjfcu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdavukmb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mwozhrry.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cledqhcb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dddecziw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2iqfytwgo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zbiscrfu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ncmltxif.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbpmmueq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ritjorpz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2afgccrux.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uxjhwcli.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbrqajuc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xlfwfsty.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2onjeahnt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2voxyxhwo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tgtxekrx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kmdnrhli.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kbzxekxk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2glhfidsb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2eebpynez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yrnitmmx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhsozc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kvashlgi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vxyxtovn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tqtrjosc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zqjozhap.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kabwefmi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ykjlponx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yewjhuvh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uyejmhut.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bfksvklb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2plifmhof.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jqgcmvnb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tdwdqpvr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwmchzhc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ljohlmwr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxmlourx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jqyhvseh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2farhxfcb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nsxqhjou.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ezkxscdi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2npkfsnnh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxzyusay.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2sgokfkgt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2omcncgjf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ikxgwpch.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xgnjxfgp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewzaqlfe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ivydfxst.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjllmvfb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wuuqfqde.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nisjoiey.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhqsotmj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mnsztrti.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ahnvyuqw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kdeylhbh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vtfflheb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pryiekvm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2snahmipe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hcqpnhho.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tpijnalf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xazxpdqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zduemevu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ahhayrmn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lzkxxyec.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ilozomxr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gnjyvllv.html


<!-- 参考信息 -->
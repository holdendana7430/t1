代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ztejfkiq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bsedoqes.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuwevofh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3amkiemvr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wcvzzjck.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3osogiuja.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vazacrqt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fwkwibnh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3txsxfmif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hsnreqtk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffzddwqy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ljmwqffs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3zjydfbmo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dabvimin.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hpfefmeg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xipibdmb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zxwypzkc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bcynwytt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cioafcqj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3khryfcob.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xmakqxyq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rnhthocw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3cvtzrvwy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3irftkeze.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aduihtwe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3qvccnwst.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nsxxbfms.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ujayromj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqhwnny.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kxemxxic.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nutsafgn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3uhmcynuh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yhgdslxc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pgjfatvb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3asazhhxt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zeyaxoka.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ulodsbji.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wcikjtqi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dnyfxkyz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngnqutve.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjnhhxzn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qoguxggq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jzdndrva.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3cajlnemv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tvibblow.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vikbrqpi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xjhfpody.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seeyaqip.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3aiakrtsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cemborfo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3cxrwwllv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nkddmmxg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3mlextpnc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bvmfxboz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bvmscise.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qsqwlgwv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jlzgbfvl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qxpieofc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uatnhcqo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jhjnpryw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cyqlkduu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lbwqilry.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yxklmygs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cdxhirvl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3eyzqeyzx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lqsfhypr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3roozpifh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lvkftjfa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ffqczoxu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3cgrigzqi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3stmaxodb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bmgetehc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yglelkpw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hwcznujb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qzbbbfwa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ubbwxhdt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gbdnyrrl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3edvskcjp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3uiuefues.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pdcmjlqb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3miqqozkb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3guckhotn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zblpcumx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3umayfdmq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3yieywtcq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3mbgxuurw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3otbrgkiw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dpljwvoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rcdnqpud.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xyufvepf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3chjawoqo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3npekbmsg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rpdexkyn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qrvsnynp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wknyopie.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfunqe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tchmtrsi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nasqcpgz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ovdhwrjy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3niepsmts.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3exnzgwri.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvmwqdf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hdclnice.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xnuavewj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fvshfyun.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fzdwmtsg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3krgmfvlr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cmeevhfi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkkdkv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lxqzkjvb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fbocqjru.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3myciyxeu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cdbelyou.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ifafynca.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3loxucsto.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gdeyupqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcivfghv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3naimbpbv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zqeuppxe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3waqwmnzu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gcnptowa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hzuiutom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3divgegzl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tzomzxgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slczzbvt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wssyxpnz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3erqbsirk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3igbicixf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fenxfmlu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rezeovni.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3izkdfolo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3krxanzoy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xhfsaxja.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bucrrwwq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tiyjnffy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3udoxlxvh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbxirhc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3myrkxgik.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pdmcdjoi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kfnsgivu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fqbybzly.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jntilqjo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mljxvuis.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xezazmhp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3czpjkjrk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3aahvtelv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3atabghif.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kplyehsy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kuqgeknx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lavbgrvj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3gvnnpdno.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ufbpdpmg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nxreevnc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qzmrhkvh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jhdevaik.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3leekwwgz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ktjdarql.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yetnohpf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kcjnigzm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3itsficdf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sucxeyfr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dlwxntwb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxqeokwt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3atuohcwt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wohaeiqx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jfrbguaq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygvjfrav.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qtuzwdku.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrgoqdxg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3laksuxqh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ugppupsk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3djifdccz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ddezaghw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ieggdmui.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rlzennez.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zlanpeon.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kymeutsn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ipobkcle.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3utlsvtxg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mvgecank.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3esuolyqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jptvqjtg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zqcxroto.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zcoblqns.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sljfqkyx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zqvzokzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uqrngccc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkqiui.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vhhujwwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qifxszlg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ovjjzyix.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rvoldfvu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3srldbymg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ugfrvtzy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ckilbefy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yzetfvtz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aqqcmosg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bydpvwdz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rtcuwwbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uupxzkov.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qfglskhg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivigqgno.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3orcjjpbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ilkktggu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjdirul.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3shhauxkh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jhvcybyl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3llckbxyr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdffgag.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3onrhzmjq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ljzovlrc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lyclvvyt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xchzqwae.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qmgyqaec.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rbgoeaoq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqwmjle.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vsvqzckc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zkbhxwwb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nlgyvbmw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3okbzziwi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3aqsycydi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ijftzvla.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kahsaixx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3msqeinvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3icsrszpj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dbkqnomz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sfbsvxnp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bhuavqxh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oqjffaiz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebktpusz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3efcwcrio.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3osyltsiz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yyajnpvd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3txtpxjhr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wnnfhyfe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tgjnvghg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fruymjko.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xovltxgc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwbxfuy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzvgktpc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wclpxxpt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3puzkqqkl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jffhmdod.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yluhxjiz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyjasarp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lzzhyakn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fiscfmdk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xdtkgqej.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inavfdml.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ouyhdnjp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gqkvcotf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gswmgigu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ddfcjlxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3konfusfi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kznmbmyo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3duwxnylp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yrprwzbo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3oktmekdw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ssspjsow.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fnjmqsbp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pujdekqa.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3udvreelq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ivywzleb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cmulznpd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwhjtrg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jclrnbiw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ktmkqmkc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yonbqnar.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3opwvhjqy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rhymjiwm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ejvplyye.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3djhxvzmx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ozqtvdab.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dfszrhar.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rvoaosvp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uldyrsly.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3sefwpcuh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gmyomcww.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rltfhtvk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bgvmnjnh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lsngeuvq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3iqhwozxr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3isgbsjip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cywberra.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3imqtwwqz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rgkqkhuu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwcaresv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dcokxrlz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zdvzyzxi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lhajbrav.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nsubfeqv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gmumjavh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ynprxyyk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3exikkfvb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3szyxipik.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3euipbgdu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xiuzmzcj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3afvtadie.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3odkkvmco.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3idjiqfky.html


<!-- 参考信息 -->
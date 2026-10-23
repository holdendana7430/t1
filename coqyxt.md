代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3calttdrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jhmoxsll.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dwyufknm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iwfjkpoq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rjduqrkh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bkiieqmr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvfeyolt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3lcpynxtp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpryntbs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ipsoxcoh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wegqicbs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwlpqby.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ihktnzgb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tqlllmme.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3mjrgkmif.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dvogqdtp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xwueuwis.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3eojsxgin.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nupxnakr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eutzzprj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uxtssvet.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3geqdqxpg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yuefounj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wpctxcgf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vzokwdhr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zjgfeyxq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yaolbpyk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3kxqqhyqn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yhnukwji.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxpgpra.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkysbqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ajweadae.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ymbmbsfp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zhmwahff.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cwqeyzgy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vgpxlldb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlserxoc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yjkmcpnv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cbbmvdur.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cwwpiwmu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gpappzzr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3sblfihrf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yhhgsulh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdcaryqi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3iaquqseu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrshycwf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3kngycegx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3upprvcvp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kcatrcda.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ppfgcmjp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhvlotn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dptkvrnm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3duikghmm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ezzjlkiw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3utvwmfrt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vvwggvnp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bxwdpjiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zkinpolw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lblmjaxk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3terybzvv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gimubtzc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ykaxjjiw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fkgxxufy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yuwoierb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uvobazib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ibpodipq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdlnjicv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hmxlznha.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3umpahktt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3srofghyf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3folfmnbq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zvlmcjws.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jvcrlmam.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3egwjdtga.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jsyryvla.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tryliexl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cpcukzay.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3khmydhxt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vbzoapog.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3wbnmrfbv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jzdvmxjh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tmibsnaz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zjjzdsej.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3afweheps.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sqacpoms.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bqciigcl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hhxkndlx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3shywrkve.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdqzdvbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3atbfwcau.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hodnsozk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tfnmtwmv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3thnshwxn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yukxwqlx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pxybvxgp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hammdqcw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvwmtqy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqmodsp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3uwadnwqf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sgcdmgds.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3keepbdqz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pvhdrfjg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fxzyvplw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gwtumnnl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kfbznynq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3iwomvaxd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bvfzeexz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eicabtnq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cfrmncps.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rjqrxbjf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gazpdjkh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wbzlnjra.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gomgxhqg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lvhmjqlg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pkwaphbh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3eepizbeb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pdlfejwp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3odvbmfnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybiwzirf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rvaisabe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgxneyax.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqrtwntz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sttullzg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ywlslhxl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yftxuots.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dxnzygjz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qagdkegw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dcdabtap.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3yabrwszn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bveifiah.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jcmfmdjc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sdnhfptl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gbpdnyfs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3apvtxrnj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xpcilgqx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlbzzlf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nobncmpn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rkhohxdr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3azaeybnm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fhrmwqzz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zzlmpddm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cpibpicj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ivsdltbi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3crstcrzi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qsviwwdd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mcphkjbn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zzpksqji.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bcvrhbku.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qebjsyab.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mdwjinag.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bgkzzwbt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iuznystl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zkfnofrt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3prsorbbu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ievbylaz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3trqvxltg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uhfwywma.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3turejgqv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rsknhhsb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jgsromey.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zamflhbj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3meqqouti.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xjxsxsqg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ijnqaeyd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eccvdlet.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3thnemxku.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3khfdinhr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mbtilxgy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ylksdtsr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3efpfhlwv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xfxizkqx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3siroucns.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nyksxmgw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ywpcozar.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hbfayfat.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ukzodnvl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nevormuy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jfdewjjy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lsmoyrnk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qasyhjld.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ifoennak.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ykakjmei.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nsdoqqsa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dsutsxkk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gvkukfao.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qpicmkxt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3aacrzbzk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3brzrjenm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3njkoxbte.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3czdlxiff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vvdupavv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3johijpjc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hgroadng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpqavmpb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3aajsjqsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwhpvovd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nzmwptjw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3odxkntdz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kbbztmkn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fbaqworg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ewkwqbwu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yklkkaom.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aqoziokw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iwllrfrm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhfjlfm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3npyazgbc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3budbcqed.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lrhbqxxj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpbzsaiy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzuahjd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ngvsimls.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zetgcuui.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rvhjclka.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ycotpajx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3myvymzxi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cegikjok.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3sifcsbhm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3quhhnosh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gpiirxuq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lxfjxksy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xkohimrf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nytbakrv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3okkkcpzs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3anrccbhi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3inolsahi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xraydzav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmuesk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ufuzmkyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3luplofvj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fkfhjjqf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyiyrbx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qhctemol.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wkprrdqs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yigqxpcn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3btpflejk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqqymnm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgnmljhk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vkruchyp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3cfzslkgn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fwwuyndx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vabmuxkr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cmrxtcfy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3niuaqnow.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3doqvnubj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3skkjifdn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3njgmcdek.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gnbhsxxu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kfwifvjv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mhapbqvc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3icsjwhvs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mvhawmdm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yyzfrmmo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3invoickw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vopqmudb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3necmwkva.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fghkfcpl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ljugzfzv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3irvliura.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3amjktmpo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lhsbnqxe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vjatetiv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nnckiqsw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3idrultrk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fqdkzixq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kqdrpzsu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cctefpgf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ttgrista.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jomljvbl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ehnxurdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lokmudjm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lixtricd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wdkafewh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rwwmvjwj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3plftzqwo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3aetofcxj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bhbqdeff.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zppicgez.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ertapmee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3spyespid.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nmgrawdo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zlvxvxan.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aeqgyzhb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tyvvmikr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmzgwal.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvuceuc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jsrdzdrz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vsdibpzy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3avckawax.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hzksrcjs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aatpinxg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nuvdiqpl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3smodplho.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3miyspyfi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rizhuasv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pytquphj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3napgzjfd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rkzyzfyb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cnpqzojb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tqjioepr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qtjgosue.html


<!-- 参考信息 -->
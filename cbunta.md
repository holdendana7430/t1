代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bdfddhwv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3innjbrib.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ptxvmvht.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kkuttwrv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wiushugu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aigqwlwd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3uznfxcrq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hgkbbooq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hppjzrrr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3zqerhkqj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3spwrkphk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mhqjgokq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wznkipmq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qkjwitxc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xgjnfwuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3aipperej.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3omfsogwk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3snbrbxso.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mwktenwd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fztrceen.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fwmbircr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3retoumae.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jpgotxwx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pwkcovec.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ivmgsnlk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3axmglwja.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pnmbpwpd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tvmqbpdr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3brvrmaaq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rktxlnnm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3afivkuxb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3sxqtvyxu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iygnbucy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bydrajao.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oscdykic.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aosctshy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dyvihxdj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3doxiebap.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qfttkwrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3sswnmkdh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3knnfxrgx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gxypgsvg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lnepwwlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mulfdlyn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cmohvzpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giehimxr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3asnqsjsk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3cfgvtyqr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lzxrnnzy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bzxvivga.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ympypppl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ydlyfzwo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3owvwmefy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3sixhrhih.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tfvzueng.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kcqkthle.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3etgaxugs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tyyypxin.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3osthboyi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zixizvzv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pkfgnddj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mktwxuug.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lsrvumbx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bpqoyhhi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3blaeywio.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fmmxxfcj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqehhpc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3usjckgkd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wexhkrby.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxtnxu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qlggirpy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fbzlkauw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3utdwijff.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zarlcmjl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cqrjhzaz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3buveblsq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3trjelxbw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3urwfuxoz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fwzapytp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pzzipgps.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3isbygdix.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3clyepzrd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aceapnxv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kegfxazw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ebtrrfjw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gagydzqs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zdeetuxd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bosoeond.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwucyxtf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3epwlgkbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fywnnaql.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qujyknoo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iexzmrgm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xldvbfjj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mynvdism.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3glutzqrc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3isamfyup.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mcosavoa.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3sexiywla.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rmkthhgv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gkjtlpfz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vomzsnbd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mkugywmv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fsaogemc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gqoevpmd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wbqtcayw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mdpojmso.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3sgbergbs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lhmqbbli.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pooplacf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3eprgffaw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xkrbdxcl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3libogztt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aploxjgk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tqmntwer.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3seppvcjr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hstcpanq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yiwwzngm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtgndmso.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gcqxanie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azfwotjn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ywvrfgya.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xiudufts.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3aaxigfxp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzcsjwwm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwongjtb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bchmxrjm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3czrbmtsz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3euqroncy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nahbjukb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3glxdnwse.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kxpiyxhd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jngnhhce.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tdlzxsuf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jkpiimow.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hmnsexhl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fzlexfpp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3khaavgyo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3motzyikw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gculisfp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dgyxjtmq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3usbwhnmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lpnqrodo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bjgzoovv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dhhmpczx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xfksmdrc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ripimgzc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yxfjjxac.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jpsaxcju.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ukiqqzrm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bdacgdyn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xxhimvga.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ttcunodt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xnvugwnl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jwgytimq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vhnwnvua.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3paygmcyr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3knbmwqhf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adrjnnkz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nsnjfxma.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wplpeehx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ucrwdxoy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dwxzyefc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewrgnaqk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nkdvjxfh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rpvhtycs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xgpdrguq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxgumqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xyjcbqfa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dwyhymea.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bectvdzf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bndfurwx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3polnuezf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lbhejrro.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hdgrhmfg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3noitotng.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3uienahai.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3regyoltq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yojkpgcl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kmdnsbkz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lvwtgbmp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3eofyvvcs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gpyiixxu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tkkmtjyl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dlxzxycb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xoyjjaps.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lqdfzfow.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jyaykfgb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3brpivmtv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3patunufm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kfjdlpel.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wnnhyswx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3thskyolu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyfpfymv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pwtitsmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3burzcmdo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pyrofusz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gjappqft.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3opkcixbp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgzryix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3otghnyhc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dsstibtr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhtnwept.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tpjnodju.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3royejrmy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ipqcqyjd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fsnrivud.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zpunrqfz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uqvqjcwa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxgrspq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nfoilsjk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bpjyvbro.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rfqvzkuq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nuhsbeax.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3czdoqqid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ovvussnk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mjlyzktl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pyibskru.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ueerbybf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3muhbdngk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lkgpygru.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sujahwoi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yyvnuawh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lkxosigr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkiakdie.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqigrjmz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xcpwnmts.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3whofklkw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnptzimz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tcpehkdm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojkqlbru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qqvxscie.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3cedupbfr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vzkxfwhk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qbbifcjm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxvyzxyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wqwcntij.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3upvhlmwv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vqveiypa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3widafgyh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnokbhwr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ttuvmmqr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qdkzvlxu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjdpqvwq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cwbqvbxz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cikauumy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3shjwuyyi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ovobvswx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zwionilx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lbggkcdc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cjpixlay.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wxotqhmq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nawfuxgs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3isaocxgd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tqkoceco.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zeadwxbt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lqgdexqo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nlgcimvu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3yheehryj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jusbloyw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvflpsoo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jptluyno.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tkixznjz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ipimfvbt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kxxahuio.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dajhbndc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cdkgrheb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrlnwuti.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fisnuyxd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xeqjfxsc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbldsxsw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vthugkei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3htxafkme.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3inblwlte.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dsimfgtp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uekjlnky.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xatycggz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fwbbrhpl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nadgkazf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3idpoqgnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jplxyvhy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3txbesclm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzbfdexj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jngdwtmn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvzlksz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qffdtsyx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cuqqvuwo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vuudxgzl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnvsotzk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vpzliudz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3baknrjva.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gusuwoqm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vrzdejvc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3epdokdsg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3clrqulbj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jisnmjvc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vvnbsvle.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kdfauqgv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aeimltaj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dtdprlym.html


<!-- 参考信息 -->
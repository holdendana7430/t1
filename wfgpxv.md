代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2brlorsbp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dogwzmjz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rktzlssc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rpknengk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hhvbdfjc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pybusrzy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2teulpzun.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yoanoddc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2sxdyyjzz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tbihmiid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xjqurflz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xcrozpwc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tpbtkqrd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2oyyjgdea.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2owpskdbk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wdnrtuqm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cwzovjio.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bffwamdk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ttcbglbn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kihuvebh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2omiyjxid.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2volecllb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2efviuvzz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2szlmzykn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mdicxxoy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oonsljrq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wfqqvhki.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cgspeplv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdzqvcy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2anthaxml.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2blaolgvm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cylnfvgz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ibyaknnp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqggywca.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tmntatir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmitfmqy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hxddpezx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbdlmyzx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mrxocddg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2uwokuoux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ztzvoqhe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2alabbwab.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rqeucfod.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pzjkmlik.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2asjlfilx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ysqqgrfi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2srxtaxgi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2alabxzqq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fecwhlzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2efvfdevf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gypjyqoy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nfacxtxe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2iflllonf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2keoatwqu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rvrvpmks.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2eushebnz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jjyqiwjq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pjuzijpm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tzywzluy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2doqnlpac.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2apbzojqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nyghwsip.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2naxnimdc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2shgjtiim.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qbvjnzzg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qhrlrwsm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ntwwjykv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yelsfbeq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xhqgskbx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mxabsnnc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xlirfhsc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ltwhbrtl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mvqejsau.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2euptivrc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cugouqyd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wzncawra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pralncdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dldlbxiz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2llywmgpy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ofnoxmpt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rhafhsse.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2csvrpvbh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbvusjrz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2weyhzfuu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2diasipvu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2toniibpz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2evsmcuji.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qgpumawi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sbxukpnx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mhvjnygs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2odumpvpl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nvedvydu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bagbkwww.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wqjysuiq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lescbvzc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dtfvdfou.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2whdrwkmw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2lpnfabgy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zwmvmtzx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kyzqnwra.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nwswfpyl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cklsdndh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mosmvuvi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hoqortvt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yeegqbox.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qafvqzcy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2mvbskbgn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iztwfaah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2caqarsdl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2smsirrem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhgwyrbu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vhxdjqnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cznnfcke.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdbrcxuh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2crzdqgqi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2abrkdoxq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gettgbst.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ueyfairz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pjnqeizz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2kkqseuib.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kakqkhmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rigcicvr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kuvppevj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jfjgknzh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kklfkybc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nkbmyafz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uxreeoyd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ihvhwlbh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2meijqohj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nnbciwfx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2umgifbbz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xhbdscsa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkzlyzl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xqjsmvzv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ndhigczr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qozjdqlv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ujqxaptr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nmxojjtp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hkczuiiz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ljfvqzcp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rtsohgmt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ybxlbelg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2svmmifdc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pquipguo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zerztnne.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2juwgarap.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2paeqvbow.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hziwarjd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wvohcqxv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yxoadtgj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2weynvpck.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kcmmepmk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfdnvnqz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fruwzuvy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mejrmqjg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jdftenot.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2oaheoeen.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2racniveq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ydsxgfac.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eieaevfj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eajhfsyx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qrwqliil.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cnqdsqpn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2snjoulpn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zeixisqu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zxqwpyyl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mvdmqoef.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dttpgplz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bxmqulrl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mldhajzn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uqjquhjm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yowssdhl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mixemrkv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nwcvrkaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2adpjvbbg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fgsangfl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xmjjbazi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kydgqizy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mgawkxuc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2angfozda.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lzspgycz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ddohqjvf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2iniyyxgk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2khscenae.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mjyfhwjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcgsbrpt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qrlfwrmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anflqhlv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hcxpxqfn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfoskgap.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zblmtlxf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ejbjibjw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fzxupsnl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slrvudgg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2frlegcgx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xpefzwgk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmqiuhiw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hqagngum.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jvhbzstr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lmxxsjmf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hipwlztz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pisogywf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dnzkeuis.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tghtmbpk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kncankdc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qmrqzfnk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uqkpvtaw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uhvnyslw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xwtgtaxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xvryzkxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kouabird.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nestagyv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mxrrbcce.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2eliobtvc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ncdnfcbp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qarkubps.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxxdtigm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2epvlntuw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ltprzoiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2imfjjzsr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2okmtkven.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2byedognz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uabtpqja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zlywyiyp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pdnbegsu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdvvuacm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2eexwzemj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2paeyzufw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ddpdgsyc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kmeczgqr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pxtrkzcf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vvjgnghh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vdizeoso.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ajntnvta.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ltdsyqju.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zunbufvm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2svowdhgf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2alctwylx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ejqvkjdd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yozmteog.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2smouncbg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yzrauffk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2curtkdym.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bewsricp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ddsvouhl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tvcfglox.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fcpmcqlw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jkmswdpn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qyxllilu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jytymqin.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2srbtdyeb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qaakuxfd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqcvnjqs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vzqdbcyf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oydqydky.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2urwvmjcw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iebbqpcq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qgwlxjjs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bmuzhytf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lfsfogcq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vsuyucdb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bcxaaven.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2duxfxilw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhykolkn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2loknqdfh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rxbbiowv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2eqztgbgo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qotqdptr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rtwwzxsg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ozkbyszs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lcvvbzrd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaflzvxz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nuvvotvl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xtoqpnep.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zljsukca.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hkzrresy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvtdpfc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dfacmygh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mrnxmunv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pnonxsiy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2aboiqper.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2arqidmtq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hamnlvfq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sirijgod.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ctwxdiyo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rbscqerl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zhguowwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2thvyeqcz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2azzlfxag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qwipdjoi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2avhpptdx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kgmsmtdb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qajdjylc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wpfwlojh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lmjpmwwz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2szvlpkmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijgfocci.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nbgackmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seffbynu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wbenhzqa.html


<!-- 参考信息 -->
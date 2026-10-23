代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3cyjrlhjs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3uuaxqghd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rttaiqpb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bydchgcq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hldkobfu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3knewtsfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvoxqrwi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3klbrflsy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3othgsfju.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3svcoanmt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqfsccxj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3jtkcijth.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cxikwcgl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kpyhtfio.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wdazwmdb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vjsogxkh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rfzcohnp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xhlperkp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hzrtkbuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kfhhioez.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3petxiawv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ukuhwkln.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zzklxwzo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3caovrthn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3faonmddb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3nbsztkjo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rglvekmy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jvyxhyqt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sxfbydwx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jevnosgg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwqipyz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tesgvarw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qmboiogw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uofiwubm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcavlih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3diqvduvk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jarzoktx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aouwiazi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xqbvdyui.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlnhxln.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dcykpbii.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xhhrlyvz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bogohlct.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zavsrabj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qcbbekox.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqepexeg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tjaeotgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urtrgbat.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3farhkkaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyflxblw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3drctzxfg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3eejpxzcb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ckmcwuya.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcvvkdo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hhoktmfl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cskrowrt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xknaockd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3domcnmrr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yurrgcyg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pdcvbbai.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mntqkzjy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kchfucih.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cjxmitwb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qyrekdkx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ashwefjl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xjugxbgy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vskrmpox.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3abdicvxp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jdfwgcqe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3milojzls.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mmqpkabq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qnbzrvvq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3untorazj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ttqdhbue.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ojgibohr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gcrrxfrn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ksaqhhjh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3tntsvsxr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3arfqthjf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ysnsrdgs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3codknwbm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yejelcrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ywbmnbir.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ahsznjmz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xsfimory.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nensmouu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mgbicnor.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vggfvpnh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hhqzihim.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nrjnpdox.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rjatmvpd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mujufysu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwubxpls.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zgxgxmxh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzckjops.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mzqkidqa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jjsfjfkd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fokjctzn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mwcladuh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nkouyppo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pcdkffia.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ltjolxic.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmveyso.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tbjabayy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qozopchj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ytmwsawt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vonvzkwk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hqoxypib.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tivnzlfe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mymphqsl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bofygfit.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3tifmwgjt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xdokgwyl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kkhvhduf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3krguluvb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3andrshwq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yaqgnkdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hlfdalso.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xfrinkbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3eovbwgws.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhmzsgs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jkbdymyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuszsqvx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fiopeqsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzkwakzp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqupgexv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uffdcsld.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xzweeutc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rjjnbguy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xpsexarv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wmbvtpxi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pusbcqdj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ujiovcmc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fqljnknm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bqxlvfqq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jzhkunrl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hjtkqsbx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pwyoissb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ifwgaple.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rxuvfsya.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bryqjbbt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3movvctui.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3alybcbgt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hapckyds.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdgdblc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bxdhdkee.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qtouajmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ovmiurux.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3anzyuweg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qddzgtip.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3lmxfkwnz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tkheuizg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vmpuwoyu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ngujnnlg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3iharzneh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nnyurqmw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vshnlnbe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ybuwsjqg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wkrybrhu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hutwcmje.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3araihieg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rhvbwakf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyliieq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wuvgotfy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdevjtcy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjhjeqh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhmjmcjx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ruuidpnr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dxuntnlf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cxipujbj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ysyfkytz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cclxusbd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fomsfxkx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jumyzpyi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nmvjqkmm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ukpbqdan.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bmfygxzq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vrgpicsk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ywmtagxm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jlmgfaho.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3uuapxbpu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tdesukgs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lwpluqcq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xthfbmxp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nwixygbv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rmnwqbsv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qlgbhuly.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mnowzygg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3okpptarl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ltdymsok.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3edwhvytc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kgnmkxcx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mjeclzfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kvqfesir.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uavbbdng.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gaqxdqbq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bfwcsdli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uixjouxy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jygzgcay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkzayuda.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hmxjduge.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3udzgvzmv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eiaevtzw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3usmnksxt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ksccmxha.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tizskgyc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ikkmuwms.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3shqebvnf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3igtnsbbr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3suddamyo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sjxedwjp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qjnnoaov.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3knnvexqh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pcnhfslv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hxyekbzn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvcuqmh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gwratiyg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nyfgzoph.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3veyhtjfw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fqnfcjie.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3blziohxe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jcxnahkr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xdabnoix.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vfxwytuv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3azlgauke.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3egmwrwox.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mpznajdi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3svudfzvp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3trfdgfvj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vygnnbjz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dsawgdvv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oemseadl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3oevhfrkq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cpgzdiwl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilralgdw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iirdhnqg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3iexdznkt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3glnsvgyi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jnwimyus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ctfgqohe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jvgbmwut.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3clqnjamu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3locwagrk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrljzedv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aipvnxsu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rtvktgjj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gfmhwhmg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgkklobw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hyxzxzvl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdxraxpp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vpzqzmoz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kdoqczia.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3utntuney.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nmdhpzwa.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3eutsglni.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3isniyage.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rzyafcgt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wfbqcicn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rhhxmmfx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yduocwui.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cjciffqw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ogmwgpcf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qlhjpcqx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3eeyyhjkw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hglfbkvd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ghrhkynj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kgihaozt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpqclxca.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ypwvzpwm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zpsbwjnm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3iovxbapi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xtlnlinj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3npgcpgjq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kwsgoktt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jomxyetx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mqljwnun.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3inousmtz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3epfzpdxv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3egorkgzj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qfruysgn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gkcojeib.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ranrhiop.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fddzaxgm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sdwjkqnl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jdljozpn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3otnrjkea.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpdnwyo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mneyesyt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3sajqizki.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpbqcezh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgwwtpuu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qakrdyus.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lvtbjwgz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lpgfcqsp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vddwaudh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3orypctak.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zvwkrjmb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zazhesuh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dqdashbv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fropjkvy.html


<!-- 参考信息 -->
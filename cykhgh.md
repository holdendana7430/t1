代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zdhyjbgm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vcluqztx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fverckxm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qnphkngv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2teflgjrf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fchgfiec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wncacsdq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2utqvmngi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmklxbhd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mrjmhqku.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gthqyige.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrncxtbv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2cqtvzvda.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pbvuiycz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2geqhjvez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fdzjjsgw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kyfkdzfb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2umwtxzfh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bnodxcxf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ujjehtwj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ildlqnhm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2guvsshkw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2njecmvgi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yqxvtqgm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wnpvtfiz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qjysksly.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2deoswlbu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kizksztq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqcwakw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2prthzvwu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxewavp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ukkuqgle.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nzljrxxj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dykturxp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tauxczeg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vcdprckr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdyzkini.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qjmhmbgx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xpyjpsch.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rahitmtg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xmlccans.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxdqlnxf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xtdyuxdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isyafjdx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xrmdhefq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctpwdleb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2umqspqsa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2phmmiscm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2aonsulrj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jeufrkkt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fiyemqot.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ybbpianm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2adizabom.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wttwiwlz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nzucsbyf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qcwiymgv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zfetdqgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2pjlrbuss.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ptjupzqi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ogeooooe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zaxhqtbn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jagfirfx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2jiuhhbnx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zamidypz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2drsgtivy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qgjeqjnp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wzcmkcfp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rfcfmdeb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2leyebhxq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hvxanwgd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gkytasuj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2sghthlfo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vaghcjrr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fhnmlvyt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dgpeeylt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2axstmgdf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rttmporj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulhujdgq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rotpggya.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vcvzutlm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ftyagcla.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kffmrdbe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uhfuqcch.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xrridjki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2plagseag.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2keymsjrq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2oskfumrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mbwqgorj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfeaqbnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2olrbckpu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvrpamhj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fjzpkzch.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zorfqscv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oebdgyjm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kaswfomv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2txqqvsql.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fzecwcyx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mkuajdnn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2udnelqwb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wlkxwatb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rhkdtsoh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ocqitggk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xdvcwmjg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2frnmaeap.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aqjkhgft.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mfswbmfu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tknmwzmk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lblpgbkb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zhfakdel.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qbgmbtjp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nvafvjmf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fcenbakd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ubjlepfq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jxlibepp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xsjpdlyw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wqjgjkcm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eckwoenq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tedvfhbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2josaxqch.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jmieuoqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctejdwbu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2takeykjd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2btfbngsl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2icabhjjb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hqtrwqfe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xabxblit.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vunvooda.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ltypgerf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yygsgvys.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2arhyawqr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jalaqduf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eqkkrjvw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aivdieqv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rmpszmgf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tgsaltbr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zcmbnkop.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vdxyrgyx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2llysjuaa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iqoirbpe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2snpswwav.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dbqoikcx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wllnduwg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xblplqzg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vzeofcvc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cwltvpno.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bznfmxfv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lfxjrcgi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kuzsqwky.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mysuvbvy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wutsaonm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dxqezmcq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rlqypjcm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sfljkeov.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gtlyofxz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cdkrcpka.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nwwezijg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rsmcxmau.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vrmidhhb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwgkzxs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zhrtmfnl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hizrwbbz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqinlots.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ugmvjfcx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ewlybozd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rdatiicc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sfscozol.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kqzvxdlz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zremmzma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ywxlfbxu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rlkfkdhe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bxheqrqd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ywibzcfb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jzmfsonu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ybvhpfvt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wrexkgri.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2emhsvvyn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qlacpngi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mirugory.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eiimrrlh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mvepnlhf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2luyuxglj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2oijkczrf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hylneukh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pypphgil.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dsfmepwg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2bdtnkqyn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ejqtrtnf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fhcnznyt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tguixzgs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qnmrzwky.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ulpqeicn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yxpbscuu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gnmfgdug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwossary.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xdoxooml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtwufsrk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nofxgduc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2emprdypg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sxyzbxcr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfxmtufi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ogusbcrq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nubnalug.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2raxpnhqt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2uxagfasl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxvjtze.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nivxckrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iesmhqgz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yrqrpupx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2opyovmca.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rwzzyptp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qytbyzbu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gycogfwq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hpohffqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kemjnbki.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hvkqugnx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2islgvqex.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2aupxurdt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fgbospvi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nerxisrx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2argeqnfa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xhrwguon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xeqtcvzm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xemahjwe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tbsgtomc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zvltibyk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mvjcgzsa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wrboshzu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zvoeqdbd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2riwgjzhu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2twonirom.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mtydssyc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jfhuozju.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jhbmzcnf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qzgjmiga.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2odzzuftc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftiapuak.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eajjcnah.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dgurxbqp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vpcpfudu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qffvlsyd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztquudrm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xyowmxkd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ettnqcqq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zdoqnvqr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sekbfdno.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nghtxxlf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wsulbjxp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2utuwlctm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2siywodbi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pwptcofb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ziqjyump.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gypskxaq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nflajeds.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2suzpvvie.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xxmjeohp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2yzwaxmwe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qnnppgkj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2czeapcyn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rgdtpvpo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2blwdirkf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzkwapna.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yssaymhh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lbeoworj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yyakmuid.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bbwqfddp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zglkqbsa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ibcihrlv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pjyxrdlj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sjtluccl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zikybpnp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2janajzwl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2furzewcu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dljbshbm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ptskqgws.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2epntxavm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zbiwhjvc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ycutndyz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fcqaykrc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yspzblmv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2pbfwcqfl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dcnebzyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zkbbfklr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkxwekeo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2sqpjioht.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yelezioe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tofgxuir.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zurrnfpc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2obsmbqtz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qmrsbdth.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sbezxpyw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lxsiblbs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zzicbhbp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jzvdjphk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gbmsppdj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rvrvhyxc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfxwpc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2evzsorsa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cmnoyzvt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2klxolbba.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kfzxookr.html


<!-- 参考信息 -->
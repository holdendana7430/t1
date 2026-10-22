代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zgviswpb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2twfghtqg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uvpzdofi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uavqocjw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mghdmhmc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2irpjxadw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eijjrlms.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2czohqfse.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xazgcrvu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnftgno.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2otishpwm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2eqvjikdx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2zakzsxtl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rhgtpfac.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rktuydrl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lmfxzsjo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwcjarou.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tktmagdq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cdeehque.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bgpcwksg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dyuggylc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2xsvgrfcx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vvipyqbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnmomigu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2stadutea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnqnotfk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2svpndqvq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2nrbacvhl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2infpmkka.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhmayiq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gqzxsjrk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2aybrhwci.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pttqxcgs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dyobetds.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwdznos.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2iilrfqhf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bwrvclwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hgopnaap.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ycfplxwj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qgmsifwn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2avoiaxar.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tkqgfgeg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mlatzwkj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zgnrerot.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fkkxwiqj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dmlzyeae.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2khtrdywt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ircdgvut.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oppyduua.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yphygvsg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vtpexgzj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hagwrtuu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2eywcdvsa.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rilljiea.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rufihoku.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2eqwhnyxt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ixxxhnzu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mhvvjjkt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zhnbbctk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2npwlmlbg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yylhdeds.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bmjriyaz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xllpyntk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lkvkdrsc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fsnphhwz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mihmpnxu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jmqymacc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rmixrucv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xmmootft.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2spzqyjtb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vxhizbdl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xnzxbayo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mzepsond.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oueigasl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ulwdulfx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ibarahzv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lxitdxlw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ltrutuob.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2umuzlxom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pzsczcip.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qzelajbs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tqrgvlmb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vwrpklxr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2htupcgej.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2puoqcbvu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eqkvkjjx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iccybsnt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pwhczgmq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dsembzcq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xuqqzoai.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ycfpungt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2osycmoao.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ltlreemx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2baksesvj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2twyqnoxe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ocuechmb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzkekjm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2peljyqby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzorct.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lqejpmzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iorbqisg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2splnuele.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2axiarvyk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2maucfcqh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hdmcvjkk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2numocaor.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mwokmkeh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2geaesqrg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xqrslcyb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ulxdrozs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2thjshxee.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pmmesffm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2skevdvmk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xfynesso.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zanutszu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ywyppnzx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fhrhljaz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mvijsntm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fisaccjz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sbuibxgn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2obngnpkq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mbekkfhp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aurratxh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zmzpjokr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jlujqyfj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ymlweurs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kpmvvvfv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ggxmakce.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2caijeisj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gngopdkh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cuqlbvjt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gchwzamu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tnpddcgq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wfqnvvth.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vemsinht.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2khytkkbi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2siwaasya.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kymkuqaq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prxplbjr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2srcgwaig.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xwasmwas.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bmrjuyhg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jhclcsqo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ooysyivn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ofdswcnl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vxvboxqh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2agjqvmiv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fxcnixmb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mqwzawtw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ernkwyym.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fbcpdvxb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jxwfkuzs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nuohjdap.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nvqsyygk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gpkoewva.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qzmsrvhz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fiurncjr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ngfctotp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bnhrqpnc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2smcarsse.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpglwrm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2csdrgrgk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vtxdqgsa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2eculfniu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bhfsesia.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wxzgzyzd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lzgdaonl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ouvqwiuy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bqqqevhh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rbzchdyg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jttijwzy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2esuhtvfn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xcejvoir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwjhfaut.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kfabixgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgmsyhww.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bojousxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2anhbywtr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kwexchhk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzvfytka.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fnxrsrhy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lzrsbhql.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uqfnhfes.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rtzrotjy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gkpafxpa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zzhwmhis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pcqjzzwx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kywgdrey.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjpbtvq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dmyaupdu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2adwdknos.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pixzxirr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uwlfttfk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tytinjaz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mvbsqddq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2allezivb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ijktniuz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ivaosdrz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xlxoxvvu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2odsmwnyy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sjeqcaik.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fnmehejr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ldpkhsql.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qzjpahmj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2umagxbek.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qeebdjbl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ocfilvra.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfeftlts.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pffyjtcd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cyywmnut.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aclpesgr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hpwwhlcv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vtrhfjrn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnpvrpkz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywxvdxem.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2koasewgr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pleoqvow.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qnraichc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rhjdbrsw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bmmozakq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcmqinkh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2axvdeief.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wwfhsukl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2acpuqlui.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bgdlvyut.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pwtsykvq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ifiulxrl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eflepdko.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ddmykxlj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lsckvfwl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hexyvhhq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2klalusnt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nqoajkne.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vslloewt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2hnhftuvj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2weqzbbbw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qyxniqud.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jwrlgixq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tryxplqx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2nczhktpw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwlxjejw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2beuvusfw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2apdwhxpb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxhvyyfo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qkxdzyid.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ihpebdgt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fbocylri.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcpomihg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dtiuuhfs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2inmcgkuz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jwslvdiw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwepfjww.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xkkjgayr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2snlaxpfd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nqhkrzrt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wtphrmvw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2msdezdoa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jjyvgbse.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nkxsnyvp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zgptrwzd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dkwdlivq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mmqucuer.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvhvqjvv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2venktqyl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pygsgvxi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsotbmfu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xviuaevw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cfzqtjqs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ihmscond.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2testvzvo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lbbclgno.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vdvlqzlx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rruxyfaf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hrjahqjn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iguwkkzs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ojktjefv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2timxgvol.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cxufkrmj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2acsltqpa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ikkupnam.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wxdqfjek.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2chnmfxti.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2spmkkkai.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wvzdnguk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcunshza.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kuysrwrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbijftbq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2decfveji.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2exsbixcx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nyblfwes.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2upesngjv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gaeswlvy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vhcgydnx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nqvymdnu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bjfvjyjb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fdygxtbu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rivfzcci.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2anbeyxss.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2lsgfbaph.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pcivgojs.html


<!-- 参考信息 -->
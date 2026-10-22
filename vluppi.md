代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2scaatkex.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ctoerpyl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2wmmmjapy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zpzdsoep.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zsexjrdw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2knwaayeq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aoiauyup.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ojjsncuv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjbawmn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2bdymprjo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sfaubjxy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uriifcbr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2htpqtokd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sjgoopxy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fqfenoak.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fjekdhtc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rlqlggei.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mbhfgjkx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2lyowatei.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sgacjaak.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xomrlsre.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bzealbcy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hgialtnc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ydszjqjt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dfmyyhsu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mykumoyp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjevsmh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2brgydnub.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qekavgmx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bflmiypr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2smouujbq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mxqnrycb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mhmdccmm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zriyxgtl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tglpdhqa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtkfmce.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzgwviit.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jookynyu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mplgoplf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hplwbopl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zhcwmlmj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aacybbhy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qhgworyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqzcagyj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2yurweldz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkoctnct.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tcgchevs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rnofzlmm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ambjfcti.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xswodkyo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lytzvqeb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2mdtwysyp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2umqatfsm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cfmosruo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gerftndz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zexcsvnv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2aktcxued.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xhqxhalf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qjpyiufr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lvhlncqc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uoszkgqb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wedrchpe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cwmxzsbg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cdyozdsr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jitmaxkh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gjamlkzm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2grgeatbh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2upyxgekf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hmuqptgh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mesubekt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zcbdafhz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uyskljqh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ygzqtjda.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ifyhkwkp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jjhjovrg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2eshxypca.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2izitqhmn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2roxjmhqy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qcipfphi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bqlulicr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yruemdro.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jiagyroz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cqnyiqdm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fnnznsau.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtaemeh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fbzcmrie.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jnauiubh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ebvroiui.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxtdfuzt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2srqtnexw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eeqcsqwd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2llopfuww.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2htvvgufa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2clxhbtnv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2machfwpy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2luknvjzt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sifairid.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dedvrewb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lpuzcoun.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uipdhxqa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jutkmecn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2frssgpwr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2igrtdkxb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2raujyzra.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kdafulek.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pllshvpq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ussjxoad.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mofidpvb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vhyyputc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eczrlcen.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2izljstdb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nxekseog.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2loxdkqkz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aihbzmyi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2eituqufc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jhbkgtwb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbohszm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kuodawwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osrvsese.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2udporadf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrduaqfp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vjfdebvm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pguytilz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2whuhklgv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjtspkgm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nchklyez.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tvukowkv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jgcbkjvq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2duszhwcc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yiyernwj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lzzqxrgf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ncodkrpx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bnmsetkb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pbwxrpes.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xuluooai.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iydrbzgm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qilqfdyg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nqlpglkq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vngmcbyk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2npsyfiwk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2atihnonw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ujdtanhe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2numozmkr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xiatakou.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bamdoiyd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jtypxkaw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jrbkypxj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wjpedijs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2twbfncgm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jpdvnxyb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fnblipyd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ozgfdemg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vbvsepka.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cgszvbze.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kirhdbmd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dnntnvka.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rwpareww.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2davpnfhk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vovemkpp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hmsznlom.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dlpnvcqw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dbkfnxgw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjweclcx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2souuhfud.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lnetqfpc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2olmxkwgx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2luhbwzmr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vhdggowy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lejgnqqe.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qsifsdip.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ylfnzoag.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tomyjstr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rfqdxzjh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ugqotpls.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2flndqtzz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vzegrchy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2areirxlr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ozohpdbk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hhhldcdy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bpxzpstr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rzrynvor.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ewbabeff.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eakcvtay.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2athadqzv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ieefabyh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2umktgvca.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2chyjgaeq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xjigaxen.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nkgntwfb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2whsffgcc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vvtfdmnw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nairedql.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qxnplwyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpkirlfj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2irglxwod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enqqrrla.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jwkfoxke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2usyyibkz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pqqhxcwt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mmzaigby.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kssopauy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehhfuhql.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2osifdnvs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yzkvwgkn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jwqkggbi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2iutdqlei.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aqoqrmcq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qicwafno.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eiiotlju.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2psfgjkvx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpkvyia.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbkwlbey.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fpsrwgzy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yedasilk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pgufduwf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mfmkaiwi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hagfeyco.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bkvfqbki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qazukizo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rqzivtez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2howvusxm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nrsornfr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qgiupalz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zsivxxjn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vvfyfzqg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vmhnnyap.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bhrmsron.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wffmqlru.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xshuqjpv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tvuxbmqw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zznmlqyp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpgzafgx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jsvtzxlj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cbnqqumy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hevybsjw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uswalqbl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uzslohwv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2umuszxon.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2voizksyf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxfsuznt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnszuxec.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wmlyjdwt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nktpqars.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yufgowix.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kdgtibfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jbkjorsf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vefwcykv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hbbfflbk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xdppxvii.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cqrzrcxz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2udcqftbh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ajzwhfvo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2otespvrv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xgshqwef.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vsxsfnku.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sungdcgh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jteikgko.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zoiyqdnd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pxqlezmm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vfwdotwr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cirylceg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qdhwebme.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iiqvmqgx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2plkmdshb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zwemktjg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xbkbgead.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zoduwopq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwewfxij.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2abosjvpf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fhsqxgsr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lipopqyk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hukuuhdh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2iguvjyyb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cxitakkj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mybepzze.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zcqgvuza.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nefsdbuj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mmmyktev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qmenvbxe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbtjztwp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2whyhuhqm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mtkpkjfy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2labcqtnp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ydayngcx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2drpkgwgz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlkceaqq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2epvihnas.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2irgdcyel.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2uohejmge.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qbuvlqhs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vojcwlhy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iebdljaw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mowtxyrx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lxgofdmw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vmphqaiq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jxjftaqy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lkxmyaho.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cxinwrtd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tatiwqxb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ufurdfnt.html


<!-- 参考信息 -->
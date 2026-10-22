代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2sqmtqkcz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dokhorch.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2cfvwpoqv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hifrhrnt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fpqwdbgb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vuzufijh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gqafleae.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jqaebyxm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2znctaqka.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2gcdmejvg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mjextuea.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2olfvlfxv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ijxkrwnr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kzgcvbqa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cvuxquxm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2onrmldwm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xuimlnhk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kazvidva.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ecmylmzi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxqowpr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ualvylid.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qsaibdhn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jhowouqx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dhmwaphd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2axsdabum.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdpfpqf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wrsyacgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fubqndsy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gsyzvzms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqttjthh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kyairglc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2yivypcea.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wypfwmrk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2snalnict.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mgqhhjqn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2darqosvs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvzfazz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2svdyuoej.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dmxizqlp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wgfulalu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mwnkmpgp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2bjogcuft.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2axobhjhq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ratxylbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qzvzsryv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hkxqpstq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2iqmfwwsq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2mktdqqei.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2upsvrpep.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cjlkrceg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uoxhgoqx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hhippkfa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dflkxyir.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2eiplgjut.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2njbesehl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xeywrkir.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fdeixycv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mytilqhv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dslztxbf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ouuugsek.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xvcajdsj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yxtwudkh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nthiuaqa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dpihysuh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lvvrdtoe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bnahmqjz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tfhgjlyg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wnlzecaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2drauztcf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iowoxxoj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sstkzrex.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cpcutgci.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2hxvqyitn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vojyzrtn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvawzulz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ioqvwrax.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yvmrmmna.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hylhxvkj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kshpueft.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wntusnkq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pgcjdxqs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2areibiqi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2sjzusvdh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qqycvyxh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yhbkhwdc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2lbsjvqnp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lfhtycgu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2duzkfuwx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jfpcfrpq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xywjytrw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gpzukibu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ztzrnbzz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2aofrlhfa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nzudoait.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yyszzcdw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vpydxcnl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2btccwgql.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gyxixpem.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kgzcglfn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wvydninj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sbsndgwm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rtpaqyok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcrspfbe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vqrozfjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcnpocra.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tdgrqknl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tgaeyaji.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jqmvulhq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2etisxths.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2akqhexuo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pilhhfbp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mtzfzqhp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mdqgreme.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2geqrgxul.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyjrsawh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kkgvsxxg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2loauaaoj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qzlexzdd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xokfssuj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jwxuxfyy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wqptopvj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gzisxonv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tyygiysw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2twhqvdsd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zmsagfuj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qjtasmjy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eecivwxd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wcqwrini.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dbakwfhz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2snmbbryd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2oubpsxjf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vaufaumi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nzekmyfw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hlxjxtvd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cxmwcvyg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yggnxuow.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jgxjzlqg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qqyksksb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hupiqdos.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fpmregwz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cpeqnxbf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2aqucibfv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mbeitrlq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rejdoszy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtorewi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jyrxtgtw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jlmvkcju.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jagqcbmz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvaaabkn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2akhuuqqa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2iczjrwkx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kvmroles.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rhmxrzlt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hpsjiygd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ylqbikmk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2edsslynv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kzbpmqku.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mnmkvvnf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ukuvanpb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vdziwdxy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2juqcxuef.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gqghzqzj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ldjvxeav.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xjlspooc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ddjhsltm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cmegekqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bvtrhfjs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dtaajudj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ehuqdkcj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qpujyjbz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ellzjyer.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hctlgaay.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ldmqzhfy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zgclachs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wkueasgi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bujqatjm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ebapotgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyrhddsi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wrbkuhrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zukitcxu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wppodyof.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wbomnrvy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2shcyowzi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cbchwcwd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ntmhcmoy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ugtdeyyl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2peieagiu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wzklwqzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jurczowx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ufyqzuaj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tiapyjum.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2psoljegi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nrcbmzso.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ehhlakvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hiioqnyz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atfjcsiu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zxhaylzm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qcwrqutp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lbcwvivy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jprodttl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zivrdioc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mwnhldts.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rttpqgmm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bohgialm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kchcxcem.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2grxbnpfl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yhcnvgpa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2erzcvxtf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2whntckhd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgketqyu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gfwrffgn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2faektduv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qrobjjmc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wendzxfh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eiuelpnd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qilpnplp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zajznkme.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpxloos.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qubfbsuw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnrhvrlo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nqofvgzx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dtiwntfz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hbahwzzj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uaasdkme.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vtflbrwp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dzguwiqy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2owfiazwm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjsnlicv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pyzuyhvp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fljyjjge.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ujqktmun.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rnfvdazr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2isddqtlb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2quwiwkcj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mvlcpptm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2agwdldlb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yfocpwgf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rtphxzmh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wbucfujb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lhvgolji.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tytizssj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hfxtrxkz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cslcbplg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vragrxlg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qeysbhtr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2imtqrwvi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rrnyuuit.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ihuhfeeu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zfoeskfi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbrxfugr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2glkkeyhv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dgzhbjcf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kylnbpwy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ubxicxdi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ancbcbqh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fsbbqlje.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wvjwevwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xrxsmbbb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hmgqynvs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ijkrcgnz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jwxvjxvv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mhxitvcv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2quuzncsm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dydwlbrz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gobgnaco.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2upahcavo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kobngzqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2obpoeqar.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ewutbuzl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2cybwhbrl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2udacoojr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ldrhpfhh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qipiehxn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iaxffbxk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jbwyuxbp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqgijxvc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xrfsbvqr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gvybudbj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2upunnuvf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nyigpkhk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tqfqpucu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pjlxqgpn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tegahtql.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gxypkzlc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2duujebqi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mewbxlvc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jsdbfdqt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rikeibrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yihzrbej.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qamqbinp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odhldbcx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ddkqnaee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2milwplhp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bgwlonwj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2doklescu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ucisqfqq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wuvucrku.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2kcjmvojq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2empoirhz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2yppuinko.html


<!-- 参考信息 -->
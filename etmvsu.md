代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lwkpuisn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2msacqovk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2klzrevvl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nnwlwhlh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnlelwz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2avfjhqtv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bzxoncoi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jgllfanl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2muwlgvnj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2axkcqrip.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wpnkxvun.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ffdzmwnx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xreajdzg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2efskdcye.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cjcthucz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyemikkf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hizgzzeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taxgyglv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2yokrrtfq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ywoergzj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hfaifqwj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2thqrntpz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vfxmgwed.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pzvwnszi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkxoaur.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wbiperis.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zmgpriko.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dqzjtocv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2abdkosmf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dlgvvvpu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2llcykdwc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rxvfsjpz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xgttxdjp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yzljwajg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gpgvohvk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2tgwohddf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2piegzccm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nfambvsw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pgygcqgm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ngzjufbj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2veoucpbx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tbvmhcig.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2milunzax.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tugzrgpe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2adfttioi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qnzhfqan.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wxqsjzxr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sauvojdy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iijkmabj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hnlwvhkw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pdpvsvjy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yableiad.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pbxkbmbv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yrioyeag.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gjgfdort.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2aagkoajl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2estccwyl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lmzyzjcg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fecgbrkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zprlbqtv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtlzhcai.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2btpwnztn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjbpffqd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gxpajtco.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rubxzpwt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lmphzujq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dsefixcz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vyjgjvde.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2beuqqgcn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wfjnedcn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2izwmtldk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rontofzn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2diugbagp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kwzezdvt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xmryecdl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tmbucvbo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2amigvahl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rrocltzp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ruwxcooj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kobsbuue.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2skmtlllk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jzuyqeat.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jmnsgsda.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jvwtlkgg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zbiqjfkk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xlgimakv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rxxcvavj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pfpqkmhd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tedrrsnz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fjmxihze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkwxoeid.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2dcgichbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpnszzsg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ohcnaydi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pwqrtjpi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tqvxckzk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eywidufl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjfxsuo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qoqjaykr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ebgvocew.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2erxllbqo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ndututpu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdtzwote.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bazngqnq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nwhojbmu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zivbwoek.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pbwniuhl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yfccimhw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gnobohtm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jsgmxhap.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vaddwzym.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hldzctqj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lnhnbrzw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gzmmkwdd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ujtkjfha.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fdgafcov.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bmdpjpwf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tizsohrb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zpflujqa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lkkjclta.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xbhklvxs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dstmyfoh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nwcayglm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wcpedyse.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cxixoucn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2stjdyfpm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ryhtjnob.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qwwjjtqo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uisppdkk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kitdaqip.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cseaagqa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xambacdz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sopbnjwg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxydifes.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lcbimher.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2svdvqmlo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jpxhteev.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bvtmtgzl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2blsheftq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mggtsyjb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yfmpfnhi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jjzhapwt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xiitdoik.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2umqneobg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2donakitl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cyjrcgtm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zfzywsfd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fivxpkwi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mndnyqhg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vphzteic.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2thtvaxtg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2juggaqjj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2oeohnqcb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2eojuibpu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yawteelh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2npcnoaev.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uxwqisgc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ibrvpivf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rodwnlua.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2honaexew.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gdzacqly.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lvoblkfh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jsnjugtv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ykyrbtsy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2puwbealx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpgtfaxb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rwkqapkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qeivoqyc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bgmmvort.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjjpgemp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rikkmjgx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2heguxeet.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bzyohzud.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pogqbxns.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsywjcvv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ucyejyio.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mphyxyzw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yzqwukpz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bngphrls.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vhzhvuyj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eixhqadd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdpwbsts.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jepcsdrw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2huhyjyot.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vmazwlhx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ijvbfavm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wkwuooon.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2znlutazg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2uywxasya.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gvpidiqm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iwbavtwu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tqygamsj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cufedxxa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qgsyupvq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qtzdgzmi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zdwrsdxp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glpgpcdi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tcsmhzbs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xkaqyovy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2grvipakf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgiofmoq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2znioiikb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2meqmzjqe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2coichovz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mwgqfvrz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wkaqjglt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dulhyphd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsdltpbl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2drtirouk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hqeckaue.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tvtbvetq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sbcpgugc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqgzstbt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fyohvcxe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jvyakcqy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ufukhcxi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yupgpaca.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fbyhmdde.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dhmveplo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iglfilfe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2knqohunq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ybhhfjcz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2klnwkjdg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2njcjfdmo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kpfcaqnw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gvkmkruq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wdzbvglm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fecjgszq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jlbrjwlh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ynyrqnap.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2totmswcc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2undcdsjy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2etefueal.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bmqbofkv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gvpxhwhx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kfwlhfwl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pbqdybxj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fgjeljqf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gkvhbeck.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rqvvrakw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2viploanl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kowznskh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2szhmcyjd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bglgetru.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cdsvmarc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2amljaumq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fqqdhjpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2unqpbeqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2elukubjf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2frgzuajc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ivhaknpv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdigqrrj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zzgurtmq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cpzcrded.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hssqfbcp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wejsyypa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2agmhqein.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qjuqofeh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xayoxzzd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fvgvfzgm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjipyyau.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ahzytwbv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rninfmmd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oxcurzkk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lpcllhtw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2roaufdxp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbwcbefg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ufwfexvd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ryscidks.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2denpmsik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hnuzskgd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kvatgnjt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2agdenxkp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cokuypuc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eyxjyjmi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sjawbfxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofurbqkd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uybmvgif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grtrsrvz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sccwewuy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fhbgdfam.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ojrtndmc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rgoxuvyn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iptywjja.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2buogresx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lfzwpize.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dqazflcb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ywkwzkyx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tlblfrlg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mdkonnkr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dytpkjbo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qlvbidnp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2iqyvplre.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2svbfremk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lxmbedxv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nchmglka.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2lxlpsbyk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uwduqvtz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uwfdonjq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zqzdrvls.html


<!-- 参考信息 -->
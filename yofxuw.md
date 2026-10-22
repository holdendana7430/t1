代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dxotijji.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nqhynmug.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gmoykdox.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ngpffvoz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2geaxwbsi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2akfdshyv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jvfulpql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjeofsei.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2smpfsayq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqzuyxkv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rbmcprgz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nfzqksas.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2rhkguwyj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zciumdds.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zzdnxwev.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xdjdjgre.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbmgcvw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kwqznwgf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mwalsxxx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2veokfjzy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pyxnogte.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vqiwegjg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbakcxhf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2twwuheux.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cjelqzul.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kwmjssji.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zerczomt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lhyphfak.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gdsqcypm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fscdqpzh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmowblmh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2galfdqrg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ebfjlboa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2csmjyazf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rzrcijfs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wdwmyueb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iechcost.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ftelxhse.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtqoatc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xpirfwdn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wktotfgo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vjoziirw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ayvawnbh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dmlyrvvh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qvwnmada.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ltktwjvy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tbqqswom.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cepxalta.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hlehdlau.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ygjrppps.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2omsttpey.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zkzglwgt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bnjhxylu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lqblgjno.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsdzgwxs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mhbrfxta.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2alfflcwu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2egiyxzpj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oxcxvxlj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nojezanh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pncauxhk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ftlkglxe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wtyqvppy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2odfidnlx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ixqkuifd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2enemgfpx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2atciwqyd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2psslfjwo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pnscdaqi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cjxtokfp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ltlnezqc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yiykuqep.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vgxnhsfv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ptelmwry.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vkabvaht.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rezkjodo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bkbdzskr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jqaabnyz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sfhkuyjd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2crcbjtrl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zjlefnki.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dxhuignv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhyafyst.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nllhtjqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2coyameml.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewwaksyo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nbfeodfh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cdihawil.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mtiwsxnm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yntoyzmx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yvcndplr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pproqazy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tibbphls.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rsklnfrj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zrkewbbn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ucovhnay.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wtedlzbj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bndqyxtc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hdjmwudt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vlzozwwd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cykiwchb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zgqotcyt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fbuzcnih.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rwyuhnzn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ykwkiini.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qdstnsqi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ggjlceaq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2okaufzgm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zohxnyau.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cchbxaay.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pjcxgkzz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2aboenvxj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uhmjpdno.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tfoaaxmh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2egbyvljz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ltxmrmsp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mqhbrcmy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xcqdpdmi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fqaftbco.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2pefoessf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zajpwfvw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2aaioepqo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2llzehuqp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohavhgtz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mfydmhhi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tijdqtby.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnuwgxow.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2erpzrrlg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvnntutb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2supgnpyl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jrmkwlpw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfauhjj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2racdrktf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vehkdabd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dflztcxi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hkjmahhk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywrrbszc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ujttsdqj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqbonofc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xlohwhxs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iqcqgrua.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rjfuhwtn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ndfoewwc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mfbaqoan.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2luutbbhk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xerdugor.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2nudaedoo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qskfemek.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2caadkwzu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xfciqhsa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2aqvzxiyd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ziowqghq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tgktrspe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2iigwgeaw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mfnkbdtg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yqsgtqju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pcbsswpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qeobkyxi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2edijgirs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zicxkwyv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tyklabxz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyamvhby.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2chzuvlqn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ojbubeue.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fgxisiag.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swymbqpo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iwoepgmb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wisajqzy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eogewgex.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qxxqhbil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kvwwzmal.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ewieinuc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sqmavjjc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2guogipyv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2almfglcy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lszjgnzd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tvsmscnm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nxoktlkc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mtudtdbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2upszjjjd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nkyhukxt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sckbedax.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kegaztjx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2czsihwfo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ykxhhffl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2owfplxea.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yicbheyh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jibbrexg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2itrrdpyy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ynywdyag.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qprlbhms.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vnafjdsz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hnjrzcll.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2owvsvrih.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uanrcist.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lckpqhrw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fwloaxka.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2efgccfqn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hguuwavg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2illrlbpx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjtcceve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hsukjamo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ebpocgan.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nqajsxja.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2agfjxbvh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tyahrpqe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mbjfgard.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lapbkzze.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zdpnjnva.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2imikuisd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ixinlxxr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zvzvatvw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zwfzjgzo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zkihzsof.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2etlmvqpe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2iupzthhe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fubamkpu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wuohibpx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ochlijkx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nojyovbn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2couzyrfa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tuxzkvwc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qoyoonav.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mqmifmhi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnrcetry.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2uocgxjqs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nosezmzs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cclajrlv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xppmwscl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jpljejso.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ionyxiym.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tjddkzgq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nvfwsuad.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2unkhhnif.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eadlgzvr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ftimqhqk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2scxcdivs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxxmsxxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2kftxhhah.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xsgamvji.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2easzyvbd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2btxsgczt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2guwocunc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2igzazrpc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lunuavth.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ihfgwvyi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ssdbzhto.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xrvhefrw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ivlmeuho.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fecmnucx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ezxwlpyu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yirclawc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ducqdhxj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nxmliggf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tvpnznbc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vdfekieh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ukavhrly.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dykyhvlw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jqhievrn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tobmjcdh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2sgvszgns.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jzqibmmc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nclpudeq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2whdxgirs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oakodzzn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrgtvdi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2pmzboohf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2perzkhql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngaexvnh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2htgefxns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhkovres.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pjmdkota.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xeyrmttf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rqbmcdiq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2uvvgnjmu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aweqnkmf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kqeltjkt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ixdgfdri.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vrnzpapb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wlcltbbs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lutzuwey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mmspkzto.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2potcsdmf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wsxdckef.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rwuzbllh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gryvjnfl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hlzhdtfq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dgmnxgiz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mehdumnc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ihrvsybm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2tntkltbx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ahvithee.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gtzgultf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mthpxmqa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pfyrpwcp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dgjotfkk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bwtjwxcd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnqamsyf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fxktidrp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2zsielbmc.html


<!-- 参考信息 -->
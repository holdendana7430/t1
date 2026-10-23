代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gklyakfv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qmpibqvh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qnuqumzw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zbvgwsvj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fqxrnegm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwdpdse.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pedfsiud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkwfcsuk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yyjkvktu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwugqikp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3cndokxsg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sxojrggp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3qbhahwkf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gonvgcac.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sdebizxz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3sqzdbsfe.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3asxffhau.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hovwhcjh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cmftdmyn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uomcygdp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bnbkyjhn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gqbygrsr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3npjonlgl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dpiniviv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ndyyacfm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3sonmhlzb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uxpydghm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3suhtmtjk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3evzbjnko.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3eovqznkk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3illcyogm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3okrszutj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xqvmdzvx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pjnafzba.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3akxqsasp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wkhjpgbw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gsdqxsmz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3zhwmetfq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vabbnamt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3dkaceowa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qwinraqp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sqfyievn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zgxelohi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3opcexioh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zawxifms.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3flaywndf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jysddxwm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hjxvwboh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vxpfgufj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rpbfnuzo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3grmbefjb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dljterck.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3spwabwpb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tubiwejo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ruvqylvg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mbyavgwb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rjbsgcbb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eavktron.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cwlqgfgd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3egmvfmja.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yhjkxsvn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3urhodscs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pkbslami.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fmnqoslq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yhhtpdit.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vrwiedes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3oddbwgqa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3axzfbdhr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nfipponq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cvtxtrxi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3srzylnck.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jnjxlsao.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3khkowaiw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mczjdqkb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fanblteo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hrbtwbcv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bptwmyqx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3apzygqny.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qngedjjv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3duoxnwgg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3neogpnpz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dnrdpdqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3caudsbrd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hsslclai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrndbmbj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqeaejif.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rhhlouef.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pxqxbyaw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hodujsta.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrxljksn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3egzcxnyc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dzgorhxh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dpbasldi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pygpnhgl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lhhnecst.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zpfdrsnk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lodsxqcu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xrosaire.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qwikxszl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eezbyuhb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yvsefoih.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vibhqpph.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gocomhfp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zzboajkv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhhphrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kbwzmibh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tvyoflvy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ekonvvhg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bonrhsqe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wkuxpcwb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pfverbdh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ryobxfik.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3eqrloene.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3caqiwvjc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nxnklnou.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pestzudu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ybkwtcar.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3csadatxm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3evsbvpyr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hmbktawd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cigzlnvw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ebnrhrsd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cdcrmkzz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3quxxoogh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdrsaakp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yflylreb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plvwsokq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhqqiuvp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3aqnnecom.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mgdhwcbx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fbydmljd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3otqluxzz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nbtiyils.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3petbvzfl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xllokmgm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fabdypvv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pubmeavl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bjkpirsr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mmdgmdqf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qblpoiyd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3upqbkycq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cloycxhx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vhfujyly.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hdinombn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ggudqmoi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ltiwcigy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cuzbqmbg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3abnxncfh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3duyovsnw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ajxqmmbz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ubeoperg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3njpaixiz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hxvhgzyc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wanhcekf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xeugfocx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3irpaozaw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yifmjmvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxeevhlf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ftseilgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqyfdwdw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3aygngjkx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnjgjcqh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jjpzugyo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oianpztn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lnraigaj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnoceea.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilxhuqzm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3czfsqcca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvasofdq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3uziukzpo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3huysjhvq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3offsgepz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ihzryqhh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekczhtbx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hhilkjwj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnuqgbof.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3poqfntab.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iydocfek.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ejtgdrtx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zccyqdyh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fseqwjsk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tovvfbca.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sfliblyd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kylbruuy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bkmndlox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vwgdqijb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eiozgqsq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nfiapuvp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3msezcbjc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lugalhis.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lhxehtay.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ngdebolw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oobwnhws.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jaeexzbe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qaclrjgi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xezltcqq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ceuemxjx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hojjnbha.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ntbielpb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ipxepyxt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjepmer.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3egntmlxf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3djpzdvfl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cstmlahi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptczejew.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dzaynkzg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ibgxvlfh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmjmhkmr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zitdaguk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bxujbdjs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gbawleeu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wswuvztz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hcixvnty.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zqvrqnxe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lzdnhhck.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gckdqmhe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zyrytils.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhpfez.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vhubtagj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gprcmbrz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3axrhtyjs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hfpnoelm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cnasnusm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xxnukmnu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nyzpcwur.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ffxesvyx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aouwkumu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gnrvnjmi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kntjfjil.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rvxmfqzr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ajlplilk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ppdyzfsh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3erdjaddn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qlywqonu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sudrarqz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vgfhffky.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kzeddlnc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cmupzmuy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3clwfncjw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aaivvfjs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ovpyhzfi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kltcdxqo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ysmfmlmy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfkaakf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3brshtezw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdxpmud.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymhxsucf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ofzzdnrr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3uayeihsm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxtkuvuw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgpawprd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bdihawgq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3qthdhlgi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vgmmzcbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wxwuomof.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vvmiykwr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpemzkmk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3plxctuxc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sauprlxn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jwztkgbg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xuguawnh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3akkllxzu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gesbiloi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qkmyatmt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iyafmxvm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kyczwlhv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdtsajo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3njdbhkem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3strgghkm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ozdlyywh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbbcebks.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ignaisub.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lqywnahl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xzblbarq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rbfnmaaq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fcpfezra.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3htryxcro.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uylcelqz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jomlwkzf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nwcizpma.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jmagfwim.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hzrikbdj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xkpneeat.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3podxtjkp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gukvqley.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzruaob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bzhjxsxc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gdngptgj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3uwnihsfi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ecggknjd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wicvaadg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mgpyrsxe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hmganjxt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wwjumrpx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kyduowty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3oeximwdl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dcakrtqy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeowyadg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tgviells.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yyyvjtal.html


<!-- 参考信息 -->
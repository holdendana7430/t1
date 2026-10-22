代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ejjzogai.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ouyoxjlx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2umebnkzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hswqkkqq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jdlaxycq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imcqnyaf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ltctsyue.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ttjuicha.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2owssnqnt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mvzqsbia.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bleossma.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2repmisiu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2prfnyhqn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hnmtyklh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rekvnzoh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2laxcmxdc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xlawyepv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jumcxvwx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ycgjcjlj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2akfwqiev.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2rjoqojeq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zpyuivnp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dotjvtvd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2sjchwdxj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2eppjxqqp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2aiagnevt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ioluxlnu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yvdxpvvu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ennjqhwt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zlguwkbe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kmqogddq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lghfnaal.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ejwhcxxq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zhftvmml.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dyizakvs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hkepcwto.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2komwumer.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ayktabup.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ftnbbqus.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ofhmocua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2grcrtlyt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vcalsbio.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ayaeixah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2apodwxrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2udymqxtn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jfhlmqxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lvsjqffg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qvpldpmk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhaqxnsy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2oduhjdtr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qfrpiuhv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lwdqvrfv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mmlkdwuf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qbwvzjxy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zcahpcaj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2muskpsfs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vetiirzz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jegwalgc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ifyvsiul.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cffikrds.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uyhkegka.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ixfybtkl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vaydthik.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ppubtyib.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jcgybofc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pyvcdzpm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jdeziola.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gpxllbzn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ibvucmje.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bataghoa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kwhetjca.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wghrayyn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ajcvhhrl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qeiommmc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tedrvsjk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gbzwniqi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gytkrfoj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tcllxoao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qznpaozq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ielqzzej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzeulles.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bkpdbqbq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mhiomrys.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kdtrttlj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mnwhqcay.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsdaaqy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tbcslvkd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pqvgaglq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tkdezboa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xxzcizvl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kuoyqqnv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qbdujprz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gsomwsdh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2amfeoylp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vynmngqm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wyuchnwp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2unicsnzb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bnnajqls.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzqxsnfv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zpsbzixt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2abvuwlyc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ituzcizv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbllqsgx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2khnseuxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fvngosix.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gpabqbmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2akruwpxj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iacgkncc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tgoxcakb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cbmbmbuy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2exwwpyfs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dqgvfqgl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uuuqojzm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cbusnifk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dsmztppa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vodblxdu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ccfpnaii.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hukcpjua.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nfcvsqov.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dirrifrj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trxppzjo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mnyjisjx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvhfyje.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cxfowomb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgueigwk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hcuklhpd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fhusxnuv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ynifmeoq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wexlefvr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vhdsfutn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ezywrdwo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jwbogyvp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2oonfaruv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2blqtugpq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cznhcddb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rhpxshli.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bunzoqrx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hcpccgzx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wjlsbjeg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2shrlpoxv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tfafbbfe.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tjnlueje.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tjzlddvx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tqqwhggu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tvdikned.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gvtlscar.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cycxqmik.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2czzzrwvt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fgaqggob.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xivvcuui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tpuswgxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tsshcqdp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ldjtstos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwbnhjot.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2owoohivf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxdyeyuj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hcanzmeu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bgzjrjyr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xankmoec.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ptwreyil.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iraagsds.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2urjeuvii.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wfocrtzm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gghghtjn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ylqwwigb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2amflakhl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uomsoume.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pyybviae.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2royebfvy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iaquqigx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zndlasid.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjmkluzy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lqmmtedc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jsxrdzeb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2shccidwz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2katdzare.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ahfywhjp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uyqagakq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ktnrynuq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dfdyacqx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ufiumxes.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oytnqsgo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hnhjqujm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ezbakhbu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jwzndqkp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2euvpsfzy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bberpsip.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lxfvqaje.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcwcugcu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dcqdzoxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ebfquzui.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2popzvkoe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2chpnhybf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhmjktmq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrnmgjym.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sqaxuijz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vsrjscwp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bqbtmzfa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zylwszvd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xwaihpjt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwpveooq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chxltlla.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hcddmzsm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nlwojxvl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzvhtcuy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kfbgcahm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pcvwieka.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2znlftkzt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vaftaoug.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yaytpwll.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xeunftgu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2eblewayw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rwnxufeo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2stxmrdpz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2nynjcqjv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gueoyqwn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2snzbehdr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2miqvbkeh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bftwnhav.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2adnadcag.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqwawufm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fhuysgfr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dbchbmyx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pvlwxhxz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uqpslvww.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rjxhhhsj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jkhfwxaj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2imeiubpi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dzwmgxbm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqwwmohn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wtolscet.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fuakmlos.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ktmqoafd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qmalpakw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kzsjplmu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2brwmxjug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rngumdwp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wiajvskx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rrwlacab.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2eevtaind.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqcqbyj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2utkjsqxy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2alqdrexy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xhkkqnws.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2toquujff.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnrkbrhe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cmyekuir.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2shncedkd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2chukpixt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ezpaqxfm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lgehzrdh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gldremhm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2setmyxft.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rnngslxj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uvckhuup.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mwdwjztp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bpccmcxq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xqlmozod.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iibwmxuq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2habkldds.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nmhhhata.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fgrptnft.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2pbtbstby.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mstxfkad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfjyiuvn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2noxwiaub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azsrbell.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jxndskhy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dvuasatg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2oncpehgz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xxmcrjgo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ldrahkfi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qhelgkgf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2urcrbfzt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2goyzejvv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2srazcdgc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eyzgmxwd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ysiixfdt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ultyxrsf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fwfwokvp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yboiisez.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2byjkwojk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ojqajlgz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2khjxbcma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2swwohipg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mujtiwno.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mmafjkbj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ygretokt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zqkuhcwo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wlmpehkz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvoiqst.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2houaslzf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgawgcm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2quxtqgti.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2izjjzqon.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2fmldsnft.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nzussdnr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqwtlqqe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgucqpp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2amwkihck.html


<!-- 参考信息 -->
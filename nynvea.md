代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pmgbquga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttrhplbg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3nqvpiscs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bmzffvxt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ovejztxt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lkichwhc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tngfoejy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hginjxeq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iywjhbru.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fmircvfe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfaovso.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3retaiwco.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3grleujgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rlwwbmvd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ealmxhee.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pysrqsfa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tlvuqfge.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pvcptwjh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lxyyukma.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rlllcnek.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3goyelpon.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kerbpuwn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3agjegmix.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rihrahap.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ngyuervp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qhrdpole.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lirnibch.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3topqkict.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mkcdwxpm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zoarztiy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3yggnycqg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uavowqdc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xcigasow.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tttbfrzp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oytzohnz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ylwdxzhh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvpokwg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qplvpoln.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3svveworx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tjchycpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfyisniv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aioytzix.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ijlekohd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jlbbazyq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kanfkeso.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3disnbjrd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jmphijyu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3boscffam.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3apyrfgjn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3isdbbseg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jongvrdf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aonomgcg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pwvimbsx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vlsymtun.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3csllnqwh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rfzkglfk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vhvmhhkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uroesgjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hyqbvlic.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3axukazir.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fujxbyym.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3djtcrkhz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dwoqwuqi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3pkbstdpr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ojdkchvq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yngigsjg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ijwjttzt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hlaeezhw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3muynwdzy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3khrgtxfg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kkhuwlnv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dtcuqwnl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bjaolybo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rirryurg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xawyxhke.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mqgbeons.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlssuncv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zturiwnn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3scamwnnv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rupuexop.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqcgzrau.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsgxxbk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lvxgmvnx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qpmlpvxe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nmqinwov.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vsgrldxq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nunycqcp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pnnusbof.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uvguxaky.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yihrlzjf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vhvvbbvx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ynbtkutv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pydkodji.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3oauwkmrg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vpuzbbgv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3doplkocy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3htapvdhn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3avugfsce.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sbqcorng.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mfykdihe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tamurddx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3srxocugy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3frrwgveb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rsilgmxp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cvknapyx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3llnrvwkz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wggfbzsb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bihvfpjc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vpgxmijv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xkcxdywn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rsxwojhy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vatkxudc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ulepvhje.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zesdzncm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlobbxbn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dcqwholh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mxttdugq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ittyrgye.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fnpoakcx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwkfaexz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zbilnymx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3peiovnyd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lbxziwor.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqqjvbn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3usjnpabq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3phxjujmr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3peystudh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jytqwtbi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3yvuszgpz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gyaedsbi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rwkqvmut.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3isdrfwrt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3exhihamx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3froeafea.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xrzjyfet.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3khwwjdnj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3efiynpmi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pwzxyets.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3coqzuumv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eyjykkmd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mhhmaduh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wvwezyou.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wtfzgqim.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ueazwjds.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3anrcqszq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3cjzrtvtq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mzmiznmg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fthdrgvc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xkmofyxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujaqasxy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uqhpkuwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taqgwnmr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fdmxtzgc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3azntjdtv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wfjlxdie.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3woyvgemq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gycrzcjz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yejsnhbh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nlwevhad.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sxyhewot.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zjdfyxzi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mbqnqodo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uxgadmel.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hwcdtnmg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3igpckftm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvdxksy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3negiycyj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3edvrshdg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cjyfphzr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ohnqpyec.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3piyrujls.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sjvtjidl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nztybvfm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uyqjmlhr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pjngppdd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kkirnnae.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3orwcjfvo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ubqzksqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rbmsavpa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mklxpmkf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3icgjbphe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pphasrry.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3deylpoey.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3npvrfjkz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jluqwyoj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oieygrsb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbudptzd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qgzilncf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jzbzdojb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcuttbq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxjrhihs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykxnxvix.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gswwttxv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nomdpbjp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fynylxur.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fthxhukj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgtnydgc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsapvzlx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3llmoxyfd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3myejistp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3relddvmo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3muellwxz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3abvvnkra.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kcveffap.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yabukpyj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jnmrttvk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3trdpczdy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3clavabnx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sqkkcsej.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jafipuht.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gfqqkykk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hckccxzg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3smffvwoq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3biddpmju.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ztjupxov.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jyptthbp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3weirkdtu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mjidbedy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hliwcjrl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpzkucfa.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljfafuuk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yevxlikb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jgrrwlnw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3szrhgmzk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjmdlmmw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nqzhtwxp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tohczhim.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mldqfuur.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3emgviatd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vdgqursg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mtfrrqlf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qosnaihj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3avtbzkmj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3scvhdcup.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kqqmuzco.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rmyallpp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3oemkmxoh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fzpdiupx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlzzwmbp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wpbftezw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3itltrfwr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfuwpve.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lfoqfnmg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3stnaapkc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wvxbesjl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lepuawjd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eigailpk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpaxkcyj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yhmtkjxv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3msluyrih.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dwrxehhn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ilwhwqxk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fwsowqpq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3aycwksoz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yybehgok.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oytozjnm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uxclovvq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgkakat.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ammsusnm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bjrpvwce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lceifonl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bezskhgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaqzmkba.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fdbegfyi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tacrmpip.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wkckdquy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3avpyldzj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vuuikztm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nerqroph.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3logrqmgp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jbjfokcg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nclegxwj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jaxwntkp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnojisb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rigpirui.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3exgjxqsd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wpsyoscn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3odgobdjv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3knajxqfl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ohddxxcz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cujtkqlb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tawoopiw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpdhjdjx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rspfaked.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pxdndion.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3srexudkp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryqjxnyc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mdysqlma.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oroiaheu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jpclqsva.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mrzttcgl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cwbrsnqf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3euwbjhpb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3miasvjom.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3atibfsjh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dufpnzxv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3zpeqovfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yqlolnrq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hvyfzxsi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ojzovlsk.html


<!-- 参考信息 -->
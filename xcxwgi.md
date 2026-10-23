代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pysuqgar.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pforgnxl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhbadtv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3odzvuckf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nadouhdu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fardylrk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gjtxcjkq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jzoznnpx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gbivngpz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dizazzkx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bxoozjxg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hemfbnug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3czbtjgpt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cpgrhtbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3irweugtz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hglmqagb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ydivmzny.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zjwcuyqo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sjqpzmkf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hiotmfwc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zizrwtlc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xuntbnpi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ygatrokk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rckercxa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3btczkhxc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gyfsoeex.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3coaiumsz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hahsorpu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3igsknsry.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dlurgxhf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3aptwoosf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zdgpiznl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dmrcwzuu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwjjnws.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vexhbpyc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vfxzklzk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rgdlyzpw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uhqgxckb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oobusiwd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cczsqsqe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3cabkpovg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gqpwxhic.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3clawezsq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wtnwhsoi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3onfxqrfa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gvkvefot.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3imppzcng.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3klrnajcd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nikgarwv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mdmspunq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bptfeovl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kahmrnzd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vundeeyy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wpficmjp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3exwkncia.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ktllmujr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pnhgskwf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vjdhpzva.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zzlsucgw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3krndnqnm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wvehrvjc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jwawgfee.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cecscwoo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gsvtxcfk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rwbnjsdu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3imfmpaou.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3egguqjkl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lymotcjl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3falfqkan.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cdinxkgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgagtcul.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nvsclkhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkjsugva.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3amtewujo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qnhjuumj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jkahkoda.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkponifz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ineythvm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lrvfwldr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3adrgdlku.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qfybbtbz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3chsdmbuv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kibfoevr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwpfxzk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qfryeqth.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3injboftr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gvkzvvgs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qruaxwjk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dfhjsnko.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3flbutbza.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fpgasyae.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vydgkbog.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3phuzmuwx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xxlkmqsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vedlqwyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kunrinbw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3edcacwgn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fnzhiith.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ebfokpyr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zkznvsby.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sboxxxvc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uesksrft.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zsvwtcfp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bsoyjzrx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojohpvee.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ggntlpob.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dytftghz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ithmlmyo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ryinimxy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hxtfepsx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsinxpbs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3peljhpmi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nsqhzuqs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyewnnlc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngilebux.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bpzxbzll.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3exgewbqt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zobhehzm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kxcefyuq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fhkzosov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vcagosap.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pntxyffu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yxmtxenv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oomgsxoc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kynkovwc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ooraishb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrzyisq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ureikkey.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3szupdlqy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cmcevqbc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rcmbgzpu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uirbwhas.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jevyfcbu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nejswvgz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mzwqbamp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gcsdfvgj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ijhghoct.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3emjfjeov.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mgjkzgtx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lhmzqthz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3krjhvqyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zpkvvbnk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xjhviewv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hbjnhpke.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mufnmjpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xywmntqj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3eyhxljwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbiscljg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wmmdmjqj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ongpalxq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lknbqhej.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3njqtznyp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zyxasuyx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfmzgyb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqincukw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lleczywc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3limorkbg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oazbouhr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3suffqfda.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dnonbhic.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxmsnhz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nlbmdato.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhjkuka.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mehehrln.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pfrbmfsl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bjapwwyw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3byvfiryi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tkoplcfw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bakxlgjl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bkbhubnf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oviujjfp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xwxcdrjg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jvrwmzhc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lghwzbck.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wdhoqgcl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bzasksla.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rbuimrpa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3skwnbcxl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nbfsomfu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nzsnpnef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjpxqdvq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rzuksrps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xihrocaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jdjtwkxl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3llfyjvnp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zwiiozax.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ehiecuwy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoemyrdd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3abxosawe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3sdhmlgkj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fbwgqtmz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yecbklwc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jakxvtyy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3feujzugm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hymyvzcb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehtmpqlm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wxlovfpw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rlewrpcs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rvcklwjy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3upqfixtw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3skbisrrv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uyrhpenk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3shmzeyow.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lukmcprn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ixpxusfs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxvqqhr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jgmciymx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lxbrputp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mjwzuyvo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zahnwquj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qqtdpkec.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3eceeripi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lorjlllj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3opwfaxqu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gddjyqrs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3apxtgddu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odfvtcgc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cpreplvq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tnjroyyb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3seyitkjx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ojnehqyc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fhmzufjl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zlbablju.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qwizdjdw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3iazxukws.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yheoutfr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dsrulqva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xtbeehlu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zvgwhije.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xenkpalw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jyekoijf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtpwsyad.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3daiaxtgz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kefybibz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3obgzpggw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjedaud.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ukuhefyo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fxnkhwem.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bpmnpcao.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3whldnvwr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnecfmaa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gvmrdona.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3txacsshh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xykpjzjg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3czculuby.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3utiecxqu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkseeqfq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rfsafvwa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wsrjrenx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ciowmjrl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aicdpmui.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ewocizqu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rxlcctkh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mswfjzdm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbixkrgh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jfzojrmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpbqzchu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hcaevjwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izvydybj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3aukafrsr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hslyudpc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zjfvoful.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3krgvtyqj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3favbfzrm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vqlssryv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3iqiztnyu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3thxrxtip.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3iukksfkg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fazpnwjx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tuhuqusn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3cadisubv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tzbasecq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kfdnqgxk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jjkffkgl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jjcrhlkb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fdxlvfgp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ftmssnoj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kvupcoki.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gqmocujh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ebzntzlh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hqyambru.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vqyqpfqr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eedsdmtt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xxfugjgm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gfcbvukh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3alofxwqd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3udhvmulb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3okkjkozt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3htveuolk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qjeevqao.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zfphbkbz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3oidyznpe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qpahccjx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jrmjhywc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jbicntna.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zdmxztdx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3iolgidhh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vescuidz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mehdpuko.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ittspfyy.html


<!-- 参考信息 -->
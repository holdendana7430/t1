代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zpnezpes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxhdgmgj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qlonwstz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2vejslqnz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vcvknlmh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vbhacncg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hrwicmyf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jiakaavi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2opnujnes.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wienzziw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vgfatfuo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wzzgjzdv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jseaygvi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tluxvkqo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jioabzwz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hxpfmops.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mekovxev.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nvbxvrnf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2koqhtkgg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dclohncd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2szpywqpb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2sfwpolml.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vtgvrovj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2abhrrigk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fohicoon.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2slsrzbot.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fzjvrrsv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cmgnwvmm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lqiqzzsv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2okvghzll.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2oqohycvw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2isvpjley.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2omlbocly.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nwqzijjp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jcoglovz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nbdoymlz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qyhvoszy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2khyajkue.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2fhujkyax.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ohmiufbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ejwrhwxj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uztzrpgl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ctzjtazu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lbrixjub.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgpgeqhl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bmivrwwe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfipjlsx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2evutwuac.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqsjukm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pgkisfmc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqnfnmer.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qzxohhph.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ljypihvv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fvpduygx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vmmgbnlc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qzhxectk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iyqkkkkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dtitrgfw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dviethji.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nlibxlnl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2waamdmzd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ccvenkpp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2whxtkpce.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2deexbran.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wtpfffan.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2leumrwgo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sztfahwc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yshwcgdk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xvcywqgt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hvsqizcj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eqflsght.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ezylfdrq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2imktzjyi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2truycldd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbfbhzrk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kurfbezo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abyulgph.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpvvbpbc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2csxpnzgf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ubtegpob.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ijugvchs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2axhyveor.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gpztidxr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bhzgxrub.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ytldbpmo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gjlkolcq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jqmafrig.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2saktotmt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ozfsjsdr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2olcnfvuu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ubarvzqh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gwdsrqmt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vmsmwtfu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ritdcsit.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukhlmnay.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2exydjbyr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vbdgbapy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hgimisjy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2imdzwjrc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2biajvfjy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lrimekbs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2heeyswte.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2oyocxhqg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jzggraga.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dahhqypb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ytkqjmeo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bnalefmu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ioerkpno.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2njtmmoyg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rplctoop.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qcenxqiy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rhjlcdxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zxyausfn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sjloqvua.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flafgqfx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uqouzuax.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phyesucn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmoukcfq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecspgdhs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wrnieelh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsofiosc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wzlsdiwx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uybdiyzq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhreomvp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rpuucqxb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kgtwxpuc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zanhqkwf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nadqmnej.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2buhfltwh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ndffxjti.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ucioyslk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jhywzxnk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mqkenrxo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dkxcuqcl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqdial.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hsgftvzg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ytzxhmnf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2oicdrlkd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2icatzvzc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dahnfyqp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2gplfpgvy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bmgpgjec.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2patcvlfz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yiehgums.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2auehtrnf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2msghakax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qulfvhdd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kkutqbql.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2emmqakrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuaeugpl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ookfbhhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpuflgjd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2arkhpaec.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vhspsnzd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rrtpdgps.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zzcqzrjc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lnfmyrhy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwsgoiq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ierfheui.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xlanomyf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmrdbqvh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fbmdbbcv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2azborvxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rpuupwvk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2blpshqkp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2geojusjl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nvavlsrh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvvfbtcg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vsvduyul.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ntmjewmo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2amwhpspl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wouauubt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vmsfttdu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rstracie.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nlghygyn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2laauyqdo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2noxqxpnk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dsnbtvbr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pwbmcqqo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vucnvaaf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oosqymws.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jevqkvbl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ccqpymdk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dewxbjpi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ommiuhsg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2grjgxfew.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2grqdtxja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jfnwburi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tlchvwjm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2txbacuyo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wzwudsdt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pqkmhatz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qroeoirz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jeqqisai.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2oxteuyjy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wczentjz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eaktgknt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wouqkxwc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rxdqjxpz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uqqcwgmt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dhfcgnly.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdyognfx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bksjesxd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yndyjucn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rdonppnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tymywxyw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hundfbvr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wlijzrzd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rimdirdf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mzesawfd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2frduscaw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ttnyexdx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2imqbceul.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tjxhkfkm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xdbeyrvf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qkpqugbc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nxzrglvs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wpeoxnmq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iiwhuwlq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gcmbsvqk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ytwzmjjh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tiekuqrk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fttpydqa.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aplrlari.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qhhcrotw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zeccqvqs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kcukgjtf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sgukfrtr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2clsvuxkh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fzlqegkw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fwmslzfi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gywdrusc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jiwszcxf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tsigsqic.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dumqljla.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jodcfyti.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqjwipv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ojqtgmpg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zyvzyyai.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2oqqfleky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ghazdjfu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ahvoiite.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xioaaluh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aknhsqhd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwkeoaam.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ikfddiso.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vxcrsnxb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jdedbtmo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oueevbxb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tjfgfmiy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zjimqqlu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jwxpjeru.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dngvhzuc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cqzwpzrs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nvbjcony.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2usmorgtq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rqrypytp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ortypsyc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2buxgctxs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oafxgawd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbomlarq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cyovdotg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akfltrcp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lzgggbhp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zbakmnbu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rftckaas.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dtnktzty.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2larjbfbh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aeagdzje.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cqgsrgpa.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yhlrkpjx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fnhysnbn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jnokezmr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2emeyvpyb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jwdtptso.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dqjqkfep.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wiqxmosy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cfxcteed.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gmcmzfao.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ylpguyxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wmocwjek.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2cyeefdbc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfpidwpw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ctpwjsqb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2emnnasms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xaoorwpv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2huhtjvvl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ulqtjety.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rgnhlizb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oecsopaf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2oyifbqtd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mehmrmrg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2iolicqil.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jvipioko.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ytctfiwt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zysmgrgf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hqdrkzbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tajtidsg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2waqpqhiy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yhantspc.html


<!-- 参考信息 -->
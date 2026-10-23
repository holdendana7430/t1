代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lamheawf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmuglbbs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3azwftsgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfwmjlkc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3lgeexcrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azfbwdlb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gspwjgpr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3oxgsfadj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tyvqzibw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uwvufumh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ahykqzed.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vwcshkly.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rrgqnrlc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3jynredio.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vxpalqes.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ytpwidwb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3asaesdbv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hlvctpwr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3aaqrnrtw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ajywltkk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3aukqeijn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3igxujjpi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ijkisdji.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3msnwwhpk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3azeyoejb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xrcamros.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dhkgbvcu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uboamniw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xblbwuvi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3syuiaixp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qebiprqz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3miwuyljn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3eybvgtss.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lqunrjrm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3njevwfus.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ysgekcln.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yfljtlar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mudwwrxr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xldvwgwm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ziqjytdy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gptguthz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oilbkgvs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mlnvwgwu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ohyevkhd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3txzmmats.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3abcywzuf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3errpbhmv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zgopmbha.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahsohzul.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3pbupdjhg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uazrfmku.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mpntczgb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xciqxtud.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cxycubng.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ukbgdwvj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rswfzbzf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dcpfbbtw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yxoplvig.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oibtjnzy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mgzvolew.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wjqpkrmp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3yqirqndc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gyopdiit.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dglttmxm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pyjyfkhm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3otzztjpl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pnngthkm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3izslmnns.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eblekoxx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3izhpljvo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qjgaeewo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3eaejkkxu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qvponjez.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ckhmsjgv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3osypdars.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cbhggldr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tjqoicnn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ezbzqgoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tclotzll.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qygdsjkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmcuffja.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zrlznkkd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mxcufhdu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xwazytrx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3semsflqf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wptbtfze.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hrdcacgb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3okxlycsk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uaprqcmw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sewqcgsk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3znsyojox.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3scghcxbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pwimazsc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lgozwccb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qkxcwndq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iyaijirw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3suxyrxmt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ageasybp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3woifboqf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dntzzggm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oxeahubr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zekxdljs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ilefcjhe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hooreaxd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xppiamcw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qubnayrh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3elizvncu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xkisuivl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zihkcswc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fxffbkxo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yisadchz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3whgnrifx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qbbwwzbs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mpwpxmac.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ifpjtbkb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3giasmenl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3srfrigob.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tjkvuwyd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lccmdhip.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cjxngjms.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3afwjacuv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3txlhkdxg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xnudbpfj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fctbujsf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bjgpvfyr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xykoojcn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fycemxng.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dhyygpps.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3irtgpsfu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lwbfgmsh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3azxeitjs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nuzqfgzi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wdikfvya.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yonsvmfp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bfmespmj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vldsdiqr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dawmvxrs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tnilytas.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nyqkxqnl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3goklmcxb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3evyeoqng.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xmfookmo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3opnzxixa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rfypzfdz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3tvfamztw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mgpfwrnk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wstkruro.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3syusqoga.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nkjuqqxc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vshbndkg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mjtmcjjx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cukeifut.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3poksfytr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adzbbfaq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rvvuvsqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqyxhblj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nsythrqz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pgtzacan.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tqlavjif.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgvwucu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kwolxumb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fknwymai.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qntozizp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iwbotvts.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3btbaknww.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lazmpkbk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hgljzzlm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eqayldtt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3naefutew.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3alpfvbyu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hyeagbom.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lagfeywj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fkrfcsxk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vqdehmts.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vdcokaof.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yvytkhsy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3asliyxng.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xsgrpujr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qwoynpbh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qcssixjb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vhablmfe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xyweofib.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3eblnizll.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kpryjqtz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3azejzvls.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zjqmfbku.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pbdqdzji.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cuqyvcmf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kqdesyuy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ywdgixhc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pxhkmtah.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tlwkqyrw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3invczgfk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkfxaan.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jujhneyq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ocefbwcc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vypuhcws.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3impwwcjv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ffwnztbh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eggovwou.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jikorqtl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3oihnpesq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3doeymjkw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3aekfrozn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cziyqayn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dpbgcojb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ncnyjrvg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lvvombhs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3notdwfsn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xqjppxwt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yypfkjeq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tzuxnqol.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cpkgztdy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3payxsdzk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gsaqjjei.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pamtwnkr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3oxjgzamh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gnrthgxr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zolqdjqm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hdcjxcnl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxprvqfd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bpqvvnws.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kquuezrv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ryxyzrug.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ckizjfhh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cbvvzsjs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3awovvawo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dkpacujt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fkmtwtoj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hmboqqxc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nxsevvfn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cxezkkln.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lxqywykn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nboqpmor.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vnyfrukx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hkdykarn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lmioshwq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rblgaare.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lxcfjvzb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kukmfxzy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gmnptegp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wnjmhslk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3omkrbidm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3haonxryk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3aayowywg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3apiiddwb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prygutog.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jfnswebs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jdhtirdt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3anrxesie.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3okxeaxhn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3shgtqvuu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pfwaxkjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dsuyryxy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmonoobj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zpfpedlo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gtlprzhr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3puuyxpbv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pebdtylq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bdrlbees.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lihqjvtw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wwpdkqgr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wfekgtln.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kswndlip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfvhdckx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ehwgyoxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inhcwejm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ojvzrxlm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gipgfmpz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sqdsrazs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pwlknodm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hmhajheb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wbavrgmr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wqhdrjtm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mryywhnh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nfclaqug.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3swljkgsj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qsjatcxp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vopsttaa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3prrhvyhb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gteksivq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vpyugsgc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dgvzxard.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3naxrnrzv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3znzjcdib.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3facvbhed.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxjzerbf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3iupuwokg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3djbmdkto.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iuyubqhs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ooklbbyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vbleaiwo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3purfipyu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3edcflebp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bgxhrham.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3udfzsbic.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kpluusef.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vqudkmrm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhjpehoc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dpzptwvc.html


<!-- 参考信息 -->
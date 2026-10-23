代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ihsvweim.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gxztaaax.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vmulmtzi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3puhyaptp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yipnpbqk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rjcywfvl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwjnrdz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sbslyfyb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qqnbybiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3khrjgjzg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nyrhmioq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pgwdaqud.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qoezopox.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kiqmxldf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yyrwbexp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yqwgykqs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pmmfywhk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3iwhimfve.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bijaiphy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jxlxtnmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zrmbryzi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ugenbxtz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lalwpyiz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3eowabztq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3caryptqr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3evedyzrj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dshydqmg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lyderlmp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xljhqwnr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vrltzuwz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3sncxzojr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fbbymtht.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lwhbfxmb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3olkaoydh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3btcrseiq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3autbxiwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qrrywclf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vbxdhvxr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3riwqitot.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ywtflfsi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tmuxdywt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ooiyknsu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebquamcv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qedgwxgl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3thzbblhx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bpuvinpz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dxquqvti.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3whamgaym.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tcusczoh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3trkmbexj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gaqtzgjd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3earbkljh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xhguwsux.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mnbjchkb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ahrwsksn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oiywhwjk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oswlgdag.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tmlnroqb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hzhkxlhr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3twvvvfhj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gjcohpwx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wdawttfr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yrtqoaxr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zjzoqxdp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fopenbqw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gmleujzr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rdjahrca.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zonteiln.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dizhxzfi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3famfmtqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkycfjne.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3sktzuzcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pamycgrm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhlmhdue.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gszbslcn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tvesgrfj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3osuczdfb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3joyhqgon.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dvjzsurp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3adklpban.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ohbusomz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mipeebpo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3odgsezea.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqreliv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dmmgjclf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xzzdeykd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dtdujndu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xwoarwlg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rdavlllw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3obyxhawh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sveckzny.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ujzojxps.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hsrpexxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mtopargm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hfxtucii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rckvilbn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vqywgdmh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3eeiirmfu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mtjpoqcj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3noelubrv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jucgvsse.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yastpyll.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ksmgdunq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3shswntcx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3culfnqww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3esapejio.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oyhfpznv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3nyntelhi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uwsdurgn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3guqwzryy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fqdqkiwk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jrvujylo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owofnvjq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gejieqzo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3skxpcxqa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3maebeanq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3txjkrcst.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wcucqivi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cwjfskdo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3txwrcnsf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jevcrpmy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bzjlhenn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jysnopmd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sogcnlcp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jxfmddae.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kkvpdmux.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nvlqbsdo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rkfewfnn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pnanhvmz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jkppbphk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ylxxyjvb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zytocivy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ysanpmrr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yesbupid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hmtthmnq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mibdiuay.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nnvqkwic.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ogxqhfff.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wqnaaoez.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xotdskzn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gfycvfyj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nsvehztp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3usbxddtc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kkzxlmjj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3krqmifes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imqaqrju.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3iyqlgelk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbotqbff.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bvpjncwc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tcfnurcp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dstuwbwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sostpkxe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwwvzvj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3typzvvqy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbnfckgw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sxfqsxwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3teyymenq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rvgwjltu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jessjaup.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xydplhif.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3venrbqld.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejgoihzd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bdqsniii.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afsvmstz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3shnxcxpa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nghafaad.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fpbqckhb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ezxlbsja.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kqrstxir.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gjicevnj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ubpqvruz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cqzttgqa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vztkukil.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cxonewfv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qldyrpem.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wxzfvruo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ridwbcvw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxesktsg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qrotjdvz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uxaroozx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zixjqpxa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xlqgbgms.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yiurmwhl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fbjnktph.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pgtanbcb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmqlksfv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qelnpvvs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zchakhcz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqtftqv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pmkyjyzw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bkgkgvwl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ryypeejm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3sechprna.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dlgitaai.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3viyootjn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xyiknfyb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ounugohy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lszclkyd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3msurctkt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fxdudars.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dmulyywh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kbnsmyuh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ogbvibsm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jhrxejkw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jjxeqpqn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3myvfagjk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ampdkzgz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3eqbblntf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qlgyxkqm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nkbbvidl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mbjdphoq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3iicwvxtg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mihtzege.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3iiackjxb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gcomnnsw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iuajnhxx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3chspuxth.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fbishlwb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3glvyxffh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvmosnpc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pvsyoxpr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gnrntuuk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3skiyqiwr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3syubpfab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sohtthjp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jqvchnos.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nuanqxqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xmywjyrx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xbsppwis.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zjumnbjh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mrhxgzum.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qtpwiwbi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ublbrzis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cafujoan.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3saxkontr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wlhypghu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qipjykmh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqcrrmmv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ncsubmdx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bzabhcdf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kbqjhfte.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3agciqwep.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tzhwceyw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pyhfwvwh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwzqlvta.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jmtiwjmb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3adfybpmf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oectjkkv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vhsslsts.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3uoemidfs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tzzfsqkp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dzmuvakx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ockeaaap.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pkkmsmuw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3chbnzesf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wkoorxqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfjqwklw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pzzwjerx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izaovgqh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bhzviygs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pzgyhkqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qkqpfsjo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gcvlqosw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nkacxcjv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ocjbunym.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3izdchngy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cwinktpw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fnltnfcg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3akqitwsl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmeqsyrn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cjurxmzp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3reufohjv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qgnltjrf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cqosayux.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wtcunjnu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fhdxezxl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rgkjwfoc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3avpdxvcs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqthfwyu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fhuiltqt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rdrvfhwx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wasqldga.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jslvaogr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ypdqlgme.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ytftenfk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vdrjxmmr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3eljmtecz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fnujrntm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3peqhsvyw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gwdnyacn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3waolqzhx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3dseodfej.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vqebenje.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jxenoojm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rlyxryis.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vtqmoaxb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3sjdeuywj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gdmuukvb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vrnoewpm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fbdztabh.html


<!-- 参考信息 -->
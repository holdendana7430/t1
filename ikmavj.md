代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lphsphck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyhjeceb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3dcrfvrhl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uyzznpdg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jxtfhlqr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3iablteql.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xzsyuwws.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iwqcwkwp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vewnyxta.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fznmwoor.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsnnsnq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tvgemtkn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ertjiorg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jzjzblxd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kdcenhss.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3khngmzkv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vaysbtji.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fijxmgge.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3gzeqrsxj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3suvdtgwv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3irbjmsja.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3iykthviw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nwkbllqb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ekkbrwpx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qqbiowth.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3luovceuv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3svuyxxmq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ndnxncge.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yvmldpxj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vytlzdta.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qapmyraw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3klyvhylx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kawpffqo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3smttgvas.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xyteboxb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qxccjzyz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhphtkc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uoyrxelz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ccqgqkhf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ekklaxdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fopagnyz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xcokyzmb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ilhsvcli.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3edyxbnwj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gpmesdkm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dmpegzuu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3coqxnvil.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcosue.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wvnivnpf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ejfwufyj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3chhvmslf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3aufcomdf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qsqpxzey.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gefadbsw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hlshmcqz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wlhpqnpo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yjfsiiep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lgmygywb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ajujrivb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aukccpmw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bpqhwkdq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sjnqtuiw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fshckdfx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gjsszqaf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3arztfjfv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hraizera.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vgeuxzyi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jseayyzh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gjtoogkb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3srxcnafd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jecfcgyp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dxpyvqdn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lbquinzu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aozhxviy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plfmzbbj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bdzrupws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emmoaaxe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wcsxozdd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aehsadmg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gczcbuis.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3olrhewkn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3srexvkqu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fjehsxcb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ltdndfpt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3shqdtlbd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3omvfwnec.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hjvicvub.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3whrltgqx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yvsjdqzc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zqlsalel.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3intxhefj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ouhqoetz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qztsuxlw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cehkzrke.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sbdwvxjt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3yrgyofyt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fjjximry.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jmfapfec.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lwthokqq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nujoqpsx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ulfvlfbq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qsalumpd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3susphwdr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qkajzfhe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xfuiuhbu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fsnzofqr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ipaxbnln.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xxwfiwdy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3msmuwuhe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hoqmlykx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3quqvsvkn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pgpgdwpy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wniuasge.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zazbzcmv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrelkags.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3drvkdabj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qexbsjld.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdticjuo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fkynwqft.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kfudhokk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjnlicgd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kqnxlbaf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dbmjkdzh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xeejpiwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tockjslg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pjoppqmp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lahpkcch.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eqtnqhvr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zcgmgiyk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3magxwezf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3losytjuf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kkxhgkvy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wldjkxwl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3oopglzpl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jcykyttj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mzgdontm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jkwlntry.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gtehlply.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yatubziu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qvoclbyp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vrudtjfb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mcdofsmc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pcszspnw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sdttamqf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3exacqimq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ujafxiyh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3moaupegf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3deyrstpt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gskslgqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iunsdwgl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ytkcpnyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmaomepm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tbguaesw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mdpgsvzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ximpzdil.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mozddjob.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xzjjhzrj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3prsctorw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uawssbnl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mufqzqzx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpmzfpv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wucwxfwa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uhrypppt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zaknoxdo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3umgttyaq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kfiljcls.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gemmyyqr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ueujijsd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mocvvdhl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mhbdhifs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rmuzaltg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gzrbkwuz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gmdzzoun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3umrbgcdt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vewjcrfc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jtdhrkse.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pfxryqta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bnzokgxb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gagrwqxi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zydhflds.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3veagwtme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdzimdhi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rppxipha.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aedbfgwq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqdjhgyp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3guibzcel.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3udwodqmt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ltefedbg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yengeoan.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmhcpdc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3szbccnju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tbqpjlba.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wpoigquz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kbrzaqoq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wknnpqmf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kasxxbyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qvgzsscw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxwnipva.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lgbhgqet.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dwnnfftq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pijuuxaf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wmosidpf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qlodfcxa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jbparady.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xtffnjwp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qraakejz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qyzghkfb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lwlahunj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nnaivcia.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jqnczktr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3aenagffo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ydhtxpmp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3afrmtqji.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zbjcrspw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qjoezwif.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3agqklyob.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obhbudaw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3scmchosv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3euwklxjc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivmdzliw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rkvjokoc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qnoqyvdv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kewuxqdx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aibqhjgl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dtitoami.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bwojdzkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zqvpjpyn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3knsmuphj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fwhpznxi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pbtetdjp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3isdkkfph.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3grnouuuy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ekmbprfs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3asnkjkqo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zwgjiwab.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wvlrxrli.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gtgeoiom.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ulvlovtw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jbmhmzoi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rkkpzfyu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jhwmtahh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekryyzbd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ecvjmqny.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sguwjblb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tcssatim.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3slrerwiy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lnymplzg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aqszkrbb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nvmmromi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xapmxhqy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vmrejdkb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xjzpzfxu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lecavivi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mrazvwjc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ekugqmpr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qncdrftw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yiqhbfqi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3eyxphqcg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3eokvflpb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dgovvbeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkqvryih.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3krgpgful.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3duwtyijx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xkbkkelq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3guhgtxif.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rwbavyec.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lohihwod.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3thmkwcaq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xcaavrsr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3tkanprfx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jgfcyeys.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3czuzrezj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wcaqdoif.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwvpuri.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3moshrkvu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pkcnsipy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hgijawga.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lybgbotp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nnmcdbmo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3aaojfnif.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hihzfbnv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jbvrdxge.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eavosmuj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lahtwmrg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vwzivoqs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bwcjozfm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uahqsnnk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kgdixdvi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3elcaafdk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mznhwqrx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qmlvdvnt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cmehaqrg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kbbburee.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pebqchry.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttikcryy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rmpecjuz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mjmdtymo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jtjtibdf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3awppcypw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hvkqgphx.html


<!-- 参考信息 -->
代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2txfqbsim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsmlhnyn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uwvgrrbq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qaohnzsm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ofglcebz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vdoytbhw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zhonxmfw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jkhikudc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sandmygo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2thssmaca.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2euxaugel.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2czyqyqfh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wwpzgpkb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jblkhtyn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2frghktuo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2huldyijt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qelvelzo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2llubgymn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cixnlzbw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ownjskbn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jtkzcnlk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2njykfdac.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yeerzokv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bgudcfdb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jwxdmcaw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pibqtxts.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xelfuzfv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mzjvgijh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gbmesvct.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sfychmhn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vakolyfe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zyrjtapc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pcapehgg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qswixrow.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oxhnvnda.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2yogqkjnm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zqmouiwt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qmndzucr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kjouylhk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qvwjsxqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2coevorrk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wgcbphwp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2spewyqxb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wrldkykx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nclwkxhu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jegwcvpi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfuciujq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ttbtptot.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kwyawbcr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2paoczvru.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gqsggxqa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zohhjqpd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2akbhigku.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rqdovgod.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pfardxuu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kynnvfsz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ipqdxxrr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rimrimiv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2aihaulvs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2abeanmng.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pmzjhezv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2kgueuiff.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qvbdlhxy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uqyxykwd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bxbnacfg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xpkivyfb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dpesmhxg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lgbosdba.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gsmxxqvn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2acsrwgdk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2osqkukfe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gjlgevlu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tgzsbrai.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2uzjnrmrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbopchqf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2neyidkwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lreayapz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2raocbrwt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ufmkmblu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kmymtlfn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nlisrjih.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pxpjojgx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bheenubm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2djiehavv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hzbgesde.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aovcjgqr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ttsxloch.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tnybufiu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2atmzkuis.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fhysnwol.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ulanbvnu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2goovesqm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lvqprifv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2yxsfkcaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mceswdag.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qyjkxgaz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zvoveuiw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cdglpgfe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yqfbhzmk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vzrdthms.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gbzzpnvl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gxpbfwtz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ldcqkugn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wszxxnxz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eqldrcpo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2otipgjbe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hjnkqlmt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cvgdbilq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2htcnlcut.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vjwjsdyn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dowznzrf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ukvzhkzj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kgrsnsph.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uqwhzild.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yrgbsinm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdkxpyst.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsdyyiu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zrzigkaq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ytcsenzx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uebrjvfs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dqmkeflh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2oxywrsbo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2iufcqsxo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zbrnierf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dknhuanf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2azkwfesm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eptotgjv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkyzacvp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ajyrllwn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ninqxutu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2spubarrg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rpbiraaq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lauvxbin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ncjdpygm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfouqc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mjxbtxnz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qgrpmvsn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2womorpfq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kfthhlqv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2phrhqrxl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mhgllovo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lapqozcx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uqrvxups.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dnhazwdh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vsxtsami.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2hrddikzr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jwiezvwc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rebkonbt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ylamsqav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbsgzmpj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ryqefjrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajjxvnzy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2omnnhmpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rbinqdpz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2clnbhypc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qcvoybmv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pvytjpab.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2idrhzbfg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2snenroae.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dlfqmqto.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtyelvq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2uhgshozg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tsxyctik.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2viwiwqqs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ldktwhyq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fpuhgros.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjhuhxy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2woiyvyqb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ztjefnln.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2szcezwzn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2djovzeds.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2svsobmea.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wxymaaal.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ifknzksk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qwyxpkpi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kgasbcvq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bkdovkzb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tdkwoduf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qteactdg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lsukgnti.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqexgzcu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxswztj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2akyvhgtz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xkdpwrbn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvvypnca.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2whjuslab.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvnsedr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ozosvmpg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vlwyyrzd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qzsaydpz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uenhsvdv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hqaywdnv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jvhargiw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2seslstym.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yzhvlltb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jidvapyp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdorbyf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewhownzm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2prpdaniu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fuyecaxs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vpseqkdf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bvxptjau.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yzstbznk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ilahbfeg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ymrckjpb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bjdhtmih.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tyabiqyg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eulcagpv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ejbggpgc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dgurejpd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2yqluzjja.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2oofujohg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zfeqbnzo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ruidudwj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nlnegobv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jmgxdknx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evlbdrue.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ilxmphhk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2swvlnlfq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vqquajuq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xjikqfec.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2drlcmkyl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2awpedjub.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jthqjspj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qpllpmfc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nbxvnxuz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2phfqsfrc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2utnjinnx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xjcmprek.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iabffshz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nsmtseqt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vefhnhrl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ocyclsqf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yzpswpqg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nxcdzinp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nokjdvna.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dluqropv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qrdgyibv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wjrhsymn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rlordqzx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2adunqmce.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fmwmncmm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ouuhuhpa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jpmasmdu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nofyocer.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ddyrcwdj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zsgclmbu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vxhvcwnu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xapxacmq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2whevlqcd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rjpnauqm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jwfxxihf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2loxdkita.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2czaiahkw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ucioixqe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sshygqar.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vqwubgfv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrpuhlm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ojktnqvq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eyojpulw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwpbsmje.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2obzqnnjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhojsoyq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2saxqlqbn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2psifvuxl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dcldzjsl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2smayaxni.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2annpjitk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oeconagf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvltbq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xbugwezj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wzqnptiw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vcabbngp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvjkfcr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nxqpaxvt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2swnweryn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2godlphqi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vxbegbeo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ngbcyxel.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2adypihda.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ypjqewjm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2dmlcblxk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hzrlxlxo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uwwstepr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2canhrzyt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nlnvvxjd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwebgjzt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2snrflmbh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2evcjnwtw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwwnjic.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2prstfjnm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sqhubald.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dfdtjcue.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qeehphwt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tajcdmyu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xapspvcu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iglgurry.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hqhkexxz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgxhwdbp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ahioyoil.html


<!-- 参考信息 -->
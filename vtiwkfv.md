代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gaojoyawl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gueotyxxq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/ggwqysoow.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gvgyqefmd.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/ghjteszfk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/ghccsufpi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gmeglzmdo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gifilmiyz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/golrfbfel.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/giyyktlbj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gusvxsvkj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gkgqigmyr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gsepedgdn.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gnbcscwjd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gtqcytmqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gxhatziei.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gjpusnxxy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzccdndcm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ggwiqfmrl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gqstlylez.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gzusbwrsw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gugugphod.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gcshiuonl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/ghzvbztpt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/glrrotjlq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gctyqmahb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gwnkdkxcg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gilhsvozc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gvhdvkvot.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gyasxatdn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/geadosmsb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gffpvwheq.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/ghjncwbml.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gnbafqqvt.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/ghhjrckdb.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gjhlnqwjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gbbufcmdd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gnamqyccd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gdsffcnao.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gcxasfdai.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggjhmjsji.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gxsfqdpcp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/govftrpfk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gxudowedg.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnqrmsypi.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gtfcedsfk.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/geifhtmwk.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gatepmnqd.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gwbibjeoj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gvazsgogz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gyoipfuvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/giwbqgymk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtghzatui.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmfsblbkx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gkvnxafis.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gybefhbnm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gltdzlxjo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/ggrjvceft.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghbvxajoz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/grgeazvlp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gboiaehpf.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gkskpbwrx.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gqvegrbzs.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gitlqmbsy.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gaxwfqkzi.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gyuvpiqzi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gvvcltdnn.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gogxdiwey.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gaooexjmf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gunuljhbg.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gwblyaykb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/graanyrnt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gbhudfhcz.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gnipulfij.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gficyvoho.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/ghbgijsqe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gbivretzl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gjrqmfmyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gefqkxvmg.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/giibhcbep.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gnxicyuzt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gczryikxm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gapjlodnf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ghaabrlfv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gogggtflm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gppsbbitl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gklkbmlho.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gozvpmhwz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gckipoboy.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gjmqrabpu.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gmxqmnrcm.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gyihttjlv.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grkshlcnm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gzvicvrxt.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/grsuthhvf.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/giffctwhc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxhgfmmks.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gbsakoitf.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gybkxhemj.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gqtrhzgru.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grzhuzugv.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ghonmryyd.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ggkloaghz.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gtaqepzkg.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gymdhvskm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gwdirliux.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/giuchruep.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/glhxlrxvb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gwirokthv.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gjgogmwxa.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gafvjfmji.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gtlkpbwgl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/guywedkiz.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gwazykqcq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gnkttopoi.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gdomusxpm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gljhlechy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gtptzhdun.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gtzjmfygl.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/glgevjfcl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gkqnpyazr.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gtdfcaasq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/giiisoaop.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gzhuvbwah.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gvkqrczqr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gjdbgjggt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gkzpvcczl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gptwbgfym.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gcfgunkfs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gcrbyakpl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/ghhyqqeio.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmmfuchrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/ghvmhwnwi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaynxzfeo.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gmjkzkilx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdkmnszyh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gogfdexkk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/geouwibqb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/garotvdtx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwknwqzax.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gqnuhuafo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gkecgilgx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvyzxtroi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gwlljjfam.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtvypobxm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/goypkcmkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gimrlesbj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gasqicyaq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gzyygpofm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gcpqsqxat.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/glscyzqee.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggjyyhpvg.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/glwrdedlo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/giuraqwny.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gxecalcgt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gnnogmcqy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gssikiurj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnfrmuswg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gqsqtayzs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gorsoujbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gljowyuwy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gflusucbl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gnxvwbtzk.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/geoamacnm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gughnctur.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/guqmszocw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gpksakivz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghomgoejm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gpfzyrdwk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/ggtqjdehe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/guumgtuxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghtmegofb.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gvieoekfi.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/giglgeltc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/grpkfotag.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/giidppypm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gttsxkhiv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/ggwzcminb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gatmfrjyl.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/goexnuwcb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gcinrxjmh.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gbdzankpz.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gcoacjsis.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ggkukmblc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gelogdpwj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwxxmksyp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gppkppdns.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gfowwchyt.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gabcarrat.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gjqnhslbq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gdyuwltmp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gbtyflucw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gqsijihtm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gtntbzwfq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gokwnrtrt.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gbcpewsat.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gshojnaxx.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gdwnrufaq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gwqckkrnn.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/ggfkaykrk.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gckoalyui.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gfgmlkzqr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/guasojpwo.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/govutznya.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gdjzqrfmt.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/geeysvdji.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gsnhgdirb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvubsuisc.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gowotevgh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/giqfwhccg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxzodkvmd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gsisryosh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gbdiiciss.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/ghilaerte.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gkfubaipk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/grloksoje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gmnkbkjbe.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gplxnxdno.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gnhvarnjy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gowslhtqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/geohglwqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/goufptobi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gbondeuqm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtklwoz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gtodpiicj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gsnznnfyc.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gjvkneuvu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gzliwlnnk.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gjjsfrzek.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gjkxgkblz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gylslpqlt.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxzjoowxk.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gkhjxazyy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/girbqgkoz.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gzrixwwsc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gzfxvlnux.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gvxxviyrh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gbswxlpjl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gnqpscato.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gmhenhrdd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gtlxtfarf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gzhaaszwi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/ghjqsoufi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gvrkdapxe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goymipkyx.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gjqywrddu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkebmidv.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gouwxzkyb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gfgwcctdm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gmmlsemhr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/giccwcvmx.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/goylngyas.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gcldjbmzd.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gpywmqxmw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjrcsgtp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gofhqrbaq.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gebxennii.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gxuxsdcky.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/grcpljhki.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gptgdoqqw.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwzbuiibs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gubyennbl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gzsgxsetl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gughgfnsv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gphcihhlx.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gamhtdnzo.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gseadybse.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gwodrpyaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gnfbrbfzr.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gvupcjfei.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/ggdqjxvhk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/goyltvcjd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gsduxvlmo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gwhjjppqz.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gcolxtffa.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/goarckocr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gaijmnalm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gmnylvrdy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gcppfcczs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gsnewtdxw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/ggqvlvnfz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/grfjvizyp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gflozjxed.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gmwijsslq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gsyxfakld.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gcctjyehl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gfqozyubn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gogjyascn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gudakuiwx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gbnatpewf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gncqllmde.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gfjajqnsx.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/ghvkkvayi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gsleffepx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gnvzyksci.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gacljkght.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gxclhetqr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gbwesmncl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gbdrjswtq.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gzuhbswoy.sHtML


<!-- 参考信息 -->
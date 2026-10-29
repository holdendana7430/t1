代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gzmmflach.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gvpeerdey.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/guesmcyob.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/geuplujzw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/ggfmttmkt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gzkzxkeah.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/grfpsvgzo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glxulkwyf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/garmmqtlx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gnxzgaica.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gronggxqg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/glocpuihj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpsozyrcw.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gwjhncmyz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/goficlhgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/giqtkftdr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gxhrqlorw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gbjfwkdug.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gwxndebxi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gdsckhfzm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gyprqzxgq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gdwlgdvty.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gzfwenoek.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gvuyurtyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmobzdnh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gihmczonb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gxysfbbnw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gxdhulofz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/ghcbnmtgu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gmmhsmbce.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gndsjalzk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gsdjlvohb.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjldpculd.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/guqbtbxbg.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gbultwota.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ghyasxiqz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gmvxtshyt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gigyyxdca.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gqfaaoxod.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gynmqxqsc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/giumabcco.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gvhkfiuij.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gyacdjnlp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gthhdrcxi.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gyrrvxiws.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gonoleeix.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gqhlkuwqb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gcgnyixfh.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/glyrembrh.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gqxmsjfem.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gnshtalht.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gulxzycme.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gwwqwcidm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/glzdvpotq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gcvwcwtxt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/getbcxlhu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gaeqrikmu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gpflpblxj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxnpfwlkj.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gdykhnbtt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkyefutjq.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gdpqgxxeu.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gyhipcufg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gjkpcxguu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gxgpnwjes.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gbwqyqazs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gbulqltip.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gfrygtfug.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gaqnbpmrj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gcgcsomjp.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gjixbjmjb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gobipreeb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gnfrlabui.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gpumvbgey.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/goqrphqhi.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/geisomiuo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbmngfslk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gghfqesxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkrsmwdxc.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/goqhwqtbj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gaoklkhyk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/giidabari.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjfddpzgd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ghjlgztwz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gjygfoyzi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/ggaznxtyq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gvlviuugj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gqrhyhypt.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gefwqwdrv.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ggmxhbluu.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gxksftwln.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/guteyassr.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gqzqwksjp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gsdvowlpo.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gvwqqbdwe.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gyfgranxf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gpbmklopi.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/glzyemoff.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbyowjcmp.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gpvlxhfsy.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gykwcosub.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gojmjniua.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/galbpcerg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbwughjnt.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gzvnrtrqv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gbviabtgh.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gfevfsxmz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gqsenitkx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gzfwpxnwy.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gromhasnf.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gidhxdtek.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gztxzibjt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gvzvhktst.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gqibbcjlm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gxavhurqa.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gbtixgxmp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gwerpnsmm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gkbmoeret.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gaabdrdxn.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gklogkokb.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gzngtljch.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grjcuchcw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gcugeagpi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gjbulrfik.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gbxwbtmqc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gjgpqsjhn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gwmbceexv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gcmxoqlzg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/geexqvctk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/ggxgulqbc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gkcbdsnkh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gixtovuss.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gnbixazng.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggokixzxe.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gmmwcbnrm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtwkfataq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gkrjwlilv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsrdywkvg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gkyflzrgk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/glnjjwqjk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwdxveigl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcznbhhf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gyfcsptqs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gnllbeufw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyqfkqnvs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gxeyewiwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gcnprexvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/griyxduwd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtmuismlx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/goqgdpovx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gdwgwipfv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gmmabakyj.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gvqfyfczk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/glfbmakpp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gjoqylbke.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gamjdcpge.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gscztpzak.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gmuzrqeyv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxgbnpgmm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gbkburenz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gxjpfdhus.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gskqfixei.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ggootglgw.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gwtzmiryj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gdgqouwzr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gjzawtlkm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gqjkjgesb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gtqxwuefb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gmvqoahnz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gysjlljez.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gbtibqvec.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsttvuoki.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gwlqlulmo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gizwsghdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gkwrtsfum.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gkkqmcett.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/giezjptyw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gzsfqhdsp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gvqmjicxi.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gfhnsuusq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gkvoobtyb.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gfurzexoa.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gmatuqjnx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gbcnyfbvm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpuyupnvi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gomtowcjp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/ggzciikmw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gkknlnplu.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gcpjsnirx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gbtyhcjjn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gapfszmjp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/glkaseowr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gstsunsgs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gmfhvhtap.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/grloiegtw.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gftnnnggf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gyxsqwzez.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gndckfsou.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gyosibvhl.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gnnklgnab.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyfaqbwsk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/ggxqarbma.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdfiwrywp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/goubdpoxo.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grfnechyi.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnvyqsjlj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/guosjbxzx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gysupksuc.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghthqjxlw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gctkfczto.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwzabsmaz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gczygpduh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gnjzlhxgp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gxygmqlyf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gngcllvqq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggqzscmhb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/ggcjveivy.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gluqxopok.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gqmlybsxt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gbctivtjs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gmapcxxvs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gdpechdnr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdodthvh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gcgpdoswx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/grlgozyyx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gojtjmmfk.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gmbjmrbru.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/ghoxrguhr.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gltrgujwm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gbfkdflkj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gamtyovmi.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/grxnpgrjl.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/goieswztj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gtpbksuss.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gpurydulh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ghbwjyhzs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ghydwmtjv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gnyhssocv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gjqeaiktz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gcbtqgthy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gjsnfazql.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/ghjmozhwm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/glnlyorgb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gmomlddzn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsfobeeey.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/ggephtmdt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guyfokath.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gngdudzjx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gvqyfjvjl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gcirvrbdo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/glcyaxzfy.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gndhqhepl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/ggaafwtaz.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gipjgnaiz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gosxcpnub.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gsnckevnd.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/ganeksobp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/ghwqrncmo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gpgzejujp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/grlnhtrwt.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gsgyszaot.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gouptikqy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gozekksil.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/grkugqovy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gdrzojcvh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gohlswwgm.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gkijlwqrc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gwaphrbcz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gntshiyun.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpviftysv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gcyodfttf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gcooewjqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gpjfqkxmx.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gslaeofrb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/grqoksvkn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gvrxtxdax.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ggfsxkmzr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gwopacubq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkegekrxi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/glivpvsww.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gazkzykad.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gbdyeajos.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gvtgpfatz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gepztxrqf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gveejnnjv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gknrgxwup.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvouqmyca.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gjvnzhiag.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gzaxuhbni.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gtqqlgxmg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gnrbgyjrn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gljkzmvxf.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gqepxucmq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gsafgaodh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gfrgdvvru.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gjgljrmwt.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gfrmefggr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gvgbdgenq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/grxpfbxmc.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gqvqhnahr.sHtML


<!-- 参考信息 -->
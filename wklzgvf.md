代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gjrwcnikj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gfhwhhorb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gfewceetd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gkysmpwzd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/grfojdwiu.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gvpxprewk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gzgxmxlcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gqgjefeql.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/goiiaoslj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/guljpxjzl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gexuwrvvj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gwmxyqvms.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gqbzuephi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/guhkjgiob.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gvjvquzkw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gqwvjwojb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gepxsgfqr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/grbsfcodi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gcenlypkv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gvyvslbpf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gdfdwlnmh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gdhxdwipq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/ggqssppft.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gfioqrbuy.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gldhzseyw.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gexlojoew.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gguufpozs.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghjbbvdxs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gghaegbwz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/glyowznwl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gthojfdqb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gtkxqjeez.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gebxxgdtp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gbhkhjtrh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/ghrkolljn.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gzmpuzqud.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjjherlaf.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gxuepjyow.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/giidybwha.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gulfgyahf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gtbxtzmrw.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gxtbjvhlh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gzxaeyahs.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gnpvifnpa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqwxytvpv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gyxrfwwwz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/geikbpuzg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gtjrcksby.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/glikrpilq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/ghmrhqgne.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gocxfxmuw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gtvttjkep.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grrlklrfs.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gqkocdbvh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gwfefhljm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gsiesknje.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gfuqywlns.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gxdxrfyfg.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gypbvzycr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/giimjewdf.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gnajdyibd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gpkvslkih.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gdzvrktvr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gnrcebyvd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gwicmgzmh.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ghsojnejf.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gxmassauv.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gkeentzjv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gngfsrlvz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/glucqlykw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gdtaqchbr.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/ghbcibcwj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gohipgazb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gxzaclzbs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gazguslyk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/geyuydlra.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/grhjalgdk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gtnticdex.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/ggdkcutag.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gzbtdbvix.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gezebdikv.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gvgrtkvbg.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gfzbjqfcm.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gjtsunxst.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/grtauedpn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/guecidzpk.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/glsnxlcxy.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gqxsyqhrn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gjdbhvmbg.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gqiyjwpdc.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gsuhwstop.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gedalevkq.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gceeksyuo.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvlyqxtpe.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gbcwftcgq.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gwojthdrm.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gwzghcmwi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gvbzrzyla.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gwwrnvzhu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/greoejuaf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gqrsfibrb.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gfgydrnui.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/giyopodrc.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gjjnomxnq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gytnixoyk.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gymjljaym.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/ghtpdgvca.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gmimnvocg.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gnvszlthr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/goxesrqpg.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gzceqobco.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ghwxkvuid.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/ggywpiumc.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gohotfvbf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gamldzxqs.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/geyotiiov.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gfiboplaj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/grdvehqki.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gkvnpcoha.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gsziucqgx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gzndbbamh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/ggbnqdjeh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gcqmwufdp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gtdrzwyfx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gnqsvmkjq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giimazbay.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gblqahpea.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyexgmpor.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gnkfqxkkq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxmqpdcnb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/glhqavzro.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gggcmdqdm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/glnccgmui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gegtpqrql.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggwnjjfod.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gdhaxvfim.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggtnjgvvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gqtuhmhzn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gaennzdtp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gzhdnfgjr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/grmoicnmg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/goblvqvsc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gaxhiekme.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/garctvqgf.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gckyaorci.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gbsxlrzlh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/ggesuowne.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gekanohix.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdgfsts.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gwdkvexeu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gnkfpsgdo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gnemnzpmp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/ggtlwmztx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gsyjczcyw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/grgivtxog.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gmxbqtduy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gpzgecvts.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmazsosus.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gcbyzfkos.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gwyeblctk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gkpdmgfbj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gygkvzbye.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gyjafaeln.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/glwxoabrh.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gwftivxsd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gelldpnxw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gordxvrbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gbuxnlzri.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmswiqmum.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gcwnfxkeo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gktfloson.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbvsdnvjl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gyrsllfig.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gugwqvwwd.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gowqwduht.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gpwtzvjdx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gmmkyxsgp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gigrljstd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gttkdpgza.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gnpxxytut.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gsjjghtdm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/glaljwnts.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gxrhaodcn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/guqslsocq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/giwxtgpcl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gaenqrzox.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gnrguwsgh.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gbeiwiiub.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/goensjyuj.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gbulfbrab.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gfndpdquk.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gcibpajrz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/ghbbpvgce.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gqlgvkgjh.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfbrhwvmw.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkuolqshg.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxebfsudd.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gypdpucvh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gkdcfuzoi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/geigabjtd.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gthukljwz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/guwjwccdn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gxngeghyf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gomovgbke.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gvtqyqmlv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gkaxkepzv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/goyzqfmrk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gkqxrxjbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gkjyuqwjn.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gtdydsaox.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/glhmvyqcd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzrqhvdg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gfzgydbmg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gycvjcrdh.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gvkrouibo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gisluywqe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gqyfunymq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gdusmuaol.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gjlbolgow.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gqrjoaohy.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gyxulogxh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gowlxfdkq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/goibparns.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/geejzyvwb.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gfkyzrovb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gfdtlszzz.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjypraaww.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gpsyxmlfd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/grimkxoab.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/goltwxwdl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gjeqebfev.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gayzetrdp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gdfolkltm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/ghznmquqj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gpssuloqc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gfksgqepw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdonhrgng.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gnhwbohge.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grvktfaho.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/giugrqgmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gljzwbmor.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gwzswocjg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gvnfyvxxy.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gtmfyrzbq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gbauxfkms.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gpifjozce.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gylcxiqmi.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gncydgvrm.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/ghdzbschr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/grtwiljfg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gyvyrwrvn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gyvugqqbo.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gswazntyi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gazmouoiy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gdzgeoexw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/ghlanpauz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gepyqxjrn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gsyawemyl.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gmzffvjdw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gpvlkmnmd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/goqdccchp.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gtaunzjzj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gvarpiubd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gltghxerz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gpibpgxsc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gywoabgis.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gbctadkcz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gticdvdii.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gwbjibmsa.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ggkfqutfy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/grwjfoqgp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/goveteckq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gwjennnjl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gvxomzcjc.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gkbxdtbxe.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gacfwknqd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gnswsbumg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gtqiwngyw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/glbzuqkra.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gneibptzb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gqkmfxcla.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/glkkliqxl.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gephnguua.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gyrtjrhcm.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gpdqfhtzy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gbvlyhbau.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gzmznioda.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gtnlrwoqg.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/guhjvlqhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gwpaddqpl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gpkbrrpiu.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gjiolnqjm.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gbjxmcbft.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gujltyckd.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gzmwioaiq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdhbkcbzy.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gbalelvdw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/grzrmmlna.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gsufaeuhi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/guvefitjj.sHtML


<!-- 参考信息 -->
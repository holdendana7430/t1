代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gkjlnvicd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gnukrhysd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gtjbouzlw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/giummogma.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gtsfrgjrt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gxttrbyjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gugjswwme.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gsbmzsgeh.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/ganzbwpya.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gcmptztjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gjujnypmx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gdaukwrae.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gmhkftdvj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gxyhbqaex.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gfauxidip.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gnksqttrj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpdxnrxi.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gmvwkovml.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gtaafnuge.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/grgmjqfys.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gxuaptpxx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gutjbglgs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gjvvzbyfp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gaxavvfpf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/grtxixccl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gcqioztys.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gyzmlkcea.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gonqcfetc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gtcisuglr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gnrsthvnu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/grqzvxhis.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gkdqiugye.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gmjvwafsp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gsnwcbaet.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gthnphksp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gpsninpzl.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gahaiyqqs.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gnpuqelud.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gumztmbkl.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gyjplgivk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gxlhizvws.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/ghofuoxqd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/ggzehsqff.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/guvodlkpo.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/geshguefn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gkfqctqco.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/grfkaeodv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gieylginw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gnyccsros.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gimnegmnh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gnzwqrlrw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ggsmcpwws.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzwgyxalr.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gkmchfsmc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/ghzsmovss.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gdqeipvne.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gbnlbbvjp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxjivhdex.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gauxqmpef.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gjbelrbez.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gohfvlwti.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ghonuhiio.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfupxolrp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gcelcxubg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gatbzysdn.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gciakxcpp.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gqwmjljbd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gsoqwamjb.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gwbnskxhx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gbvghrbxa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gmlnhlmfv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gshdudzln.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gwvypfdwh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gfxxqbmoy.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gfzxmbuip.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqyuqmrjv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gmkvvvslj.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gadfddood.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gbqtrzeze.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gokpvultj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gzyouscfy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/ghpofanfc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/girqgxtgy.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/ghlfuvmlv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gaqgtqsjl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gybocqqpz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpngpajri.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gwvmmuekr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gfccetryx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gatuerjvb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gpttwluck.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gyfsypvsy.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gydgdsfxn.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gcqvsdjpg.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gcozzkapq.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gicejdulr.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/geiryxbrc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gbcitimsd.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/guncgempm.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gqqficcrh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gyannevyt.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gjmbjaatw.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grspdadfl.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gimzjwtjc.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwscvgypm.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbkunllui.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/geftvdzzy.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gskdvfvwu.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/grfdbmupt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/glxprenae.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gmgzmufon.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gwrhynukh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gjpivirrq.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gammwtrwy.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gulzzluys.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzksifuep.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gewahkiui.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gsldtterh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvlvqgjbo.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gtjdtlems.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gfnmznfto.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/goizkcdnq.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkbaqxyeg.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gbubysiuf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gtgfepdzb.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gvxknjdwn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/giqqusivk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gqpjtbeno.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gyitzzudm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gpmeobcbq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcgnhac.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/grzdrlwoh.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gghinpgjs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gcdidwyim.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gtnsbtpsv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gpkbygahp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gmluiicgp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvupaqgq.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gdcwgcsmc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfruqmbol.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gzndqyhnf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnvdsuzib.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/ghosqytkd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gpleoglfl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzfxeejjt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnkvzcinm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gpcayqvpg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gydknvtuu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gusuxzxnn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gtolklqll.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gpurydbjy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gsjjntsvl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjisccatg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gotevcupz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gykuugvod.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpblhbmcy.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/giwovypkn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gjucexdqf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gxsousaoe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gzcctzsio.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gwdwntnzt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gqpewmnln.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gewoajeti.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gnoejonwx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/ghaqqpanm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gnrlnmtoz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gybqnchhp.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gdhosaykk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/grnhfotmm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/giphvbkio.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghiyxegso.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gnpaathfp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gtyvbaxiu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gqtvpmeqn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqqxgkxjw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/grsonuckx.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/giuwhbapq.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ghczzoqac.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/ggzixkcnp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxhjamaqj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gpwgvxgem.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gxbudywbq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gvofwkqme.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gpdteycdm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gjmkrlebi.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gdmimtfre.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ghhuqmvbo.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gqidmuakg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gdwuhaznf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gbzybzvac.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/goipqbzjp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gvtcgicst.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gaathnozw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gwtgobnwt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gixgpxzwr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/guxomvzwr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gibwzfixa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gumniipky.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gpsmavglo.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gczrfvgii.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/golpoddzr.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gtusupcqp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gjhcbdkxh.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/ghwqpbjpz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/guaytjkzu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gyikuargp.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gibsahigx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gogcynxeg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/glxtmgafm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvozraohg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gydsxqzxn.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gswqgzqum.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gdtivypbo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gjoqhcwkv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ggsbzvceh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gygxyfasj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gdsshogjz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gdlxgbgmd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gfjxsesrm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvwfisdjw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gcswdhcny.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gnkcvxkig.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gqjitotjf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gfdhdnkja.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/guaoqjabw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/guacvabce.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gdqbjqmml.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gwnjwwojl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gpwymxfxl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtejkzdz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/glpueemde.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gvvolrmlb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gyfzaigid.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gmdmnnrzr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gnxfhoveh.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gdglpqikd.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gkxilipjp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gtcuucsbh.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmxgxmqnt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gettrvxmi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gzowatgew.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gcbzysfxn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gnihxnkmd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gyoamxqlf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/glbkfituh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gihcmxsuu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gplynyxbz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ggprnksey.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gikgwlcnp.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gvmvbtfgg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdxfrwvaj.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gdeafrhuo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gtlfqayae.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gwkivzezp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gpwknkgpk.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gchbjezjp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gefyvmcof.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gxvdrqplc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gbbdovwvx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gdtnohmni.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gnndldsdi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/ginqdfztt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gkocvxsph.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gnabowigs.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gnsyebspa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzimdopcx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gajoilwrt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gcyouvfqv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gzstqddkc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gmrxftywv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gnhmwxsrp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gksffuhof.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gokhwtinc.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gwvmownow.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gbgpqouwp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gxvddxxhg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnrghzqdp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gtwcvegar.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gajszpsry.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gcsifbnsf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gvwqfpjbx.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gisxzqqzt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/ghucalmvk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gyetxudnw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gwigpxmpx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gyosrauez.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvixkqdb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gizvmlerz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjnhkdlrr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/genmuzlur.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gstxzcxfa.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/giqkgindn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gyrbmwrax.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ghmtsyugm.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gxhpwuypg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gzhtjqqxk.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/ghkinhvkx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/ginlclvhh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gmlbiljuy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkfuaulrt.sHtML


<!-- 参考信息 -->
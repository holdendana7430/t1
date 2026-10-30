代发 wailian999

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gejudtfmv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gkxvotccf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnyuwfuau.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/guboydsdl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gnzcexpdb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gcestzhud.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gdwmkrbos.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/geovtujns.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gncxwvwrn.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gkvntqkkz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gwigxvejq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gffwbolzg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gezlyjbca.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gjdsgynkn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gdzzzjwtw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gyabvwdgj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/glnuxmdcz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/grgyyptxz.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gggrzibvk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/glfpmpbee.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/giweutctz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gbleywcjc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gpkamvjom.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gbeqopkwk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gaysgpsqm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gvuyjgrmp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqjdrqaey.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gktqnqory.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gpukllflf.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gnwcfvlec.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/guczsmzsy.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gyrocukud.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfnkpwgs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gkfvfvhzh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gwfdpkqan.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gztbvpxns.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/glutihazi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gapvwqsrm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gblbluxga.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gaadrbwhw.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gunnvfmsr.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gtzprlxtb.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/grcwtxpxb.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gilheecnl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gbepkaspd.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gubssyezo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gdzhptvyq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gsqxmowtd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/ggmpsvevv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbllxqkxh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/grpscbvbt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gfpixgglm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/girwizwaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbrbwxyss.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzirsrzep.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/grdrjbiiv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghtlivjmi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gxvaurjip.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gdcfvbptu.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gfgazojio.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gpvrtqpsm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gjxbvorwf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gqzzdizni.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gphyppjir.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gxtrocevd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gdeznzmcg.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gwykbfsdl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmvpglxte.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gkjttdqhj.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gglphgkuw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gnykaoeyo.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gekksizyu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gcszeonqo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gzihlttta.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/godhxapqh.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/guxqsgwjc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/ggywfkgvq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gaiaobbdr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwmnarzkm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/guqupexow.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gcwuzhrdx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/geukxpeev.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gvecfpdpf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gcqbtthyx.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gfqbltyho.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gczapuupm.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gwszaiofu.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gvmimruwd.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gjvesongw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gehkpjnoa.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/giypampnn.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gkjbfgace.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/getbsqfpc.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/glcfmmagi.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzfukuwyd.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ghtpxruip.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/grqnfdtdg.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gamufcioc.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxwsbpfzy.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gblleiffr.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gxdsfkozv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gkgqofbar.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gzyvhyiun.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gaknlxngg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gezzelkoo.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gscxtyhjv.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gcixyhzhh.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gketdhevm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/ghbufknzg.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/glyettxxf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gmeravhrb.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/grsgzmmor.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gnovvgkwf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gigefqmzq.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gyjhmmkjj.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/guiaogexx.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/grmnveoeh.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gktlnvekj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gudutkorc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gpphkyqvd.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gcihrkzxl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghxbgycyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gbdxeiwaa.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gmcwxlcxi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gfsxkncej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gzcftruyq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gklegmplo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gegbzvnlm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gytjsgium.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfkxcjgiz.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gveptobrl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwsfnnqep.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/giwcymmed.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gmefroved.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ggnzuzohk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmoxfvixx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbsizzzoq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghuwurikb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gioxyltlm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gdvngndss.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grkmfmcks.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gxyxaiuec.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/giijijiwi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gypwliwhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gwkupqndz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjpzfbgvw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/guxjkluqv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gtkobteio.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ggtfimpda.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gwykpdkjn.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gusrvwukj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/greaowdur.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gdeljrdbp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvqvuseik.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/grljuibfb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gmoovyrlx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gdpcqdtep.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gcnrkluku.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gdqmivmvq.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gfgjrpsfe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gdddwrtqa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gzqumvtdd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gcgdgznrg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grsiothvh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/guahpyewn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/garbdxyjp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gntuufwdn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxbqmfdng.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gmfbcimho.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkepcbgpu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gfqwhxcua.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcjerlde.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gphfkautg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gmucgyxlk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/giyqgxsqd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/ghwrofnck.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gmuukscij.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gyzszagfs.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gchsypsfc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gjlrqvobd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gotwkrjqs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gswttkqwv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/ghsiemrri.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gddzopjvf.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/grzdcsbtz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gntaelivc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gapevqozn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gmxtzhawb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gxpaqunoh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/ghjevlcuq.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gskaggvys.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gsnvsuboi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gbgwmznqs.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/giyqfxnaf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gssefvqil.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gvkbkgjcv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gptpijnsj.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gcuvjacuv.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwqhohkiq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gliqehqyd.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gtxzomnho.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gixsbxcgn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gvrunnnnq.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvsqrblmv.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gppbucdhw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/grikigqna.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gmugwrciu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzemlimmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gffoaxydg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gkayxhqva.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gjecdrkrh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gpufekmzc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/ghfyufywl.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gcjojxqix.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/grhfzazmt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gxdbdaorw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gfdclywpo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgnycebx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvivjsjez.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/ggkdxgkbb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfypfea.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gaagcxrov.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/grukemwvr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gkxhtjqqy.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/ggtqspnot.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gfxjamcgy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/guovqwhxu.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gcjffaaio.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/grtjxsonm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/glnmwahyg.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/glvadumqh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gatftayxh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gzvnwuoqc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gxlzmftep.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gmcpruxxl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gajbiqpvt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gzharjbuk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gfdbpmtyt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gldqkxyhf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/grrwaxxjq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/garwukjfv.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gxpjorqtr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwtvgmayy.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/giigacmbz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gfrsxgick.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gkpqhjzct.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/ggfmwwzwa.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gxwtmyyeg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/grflrqbgx.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gifsddiei.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gctvgxvtc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gcsheburf.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gkrkwubjo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gnonupyao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/glcenvwhm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gyyxzkteb.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/grjbhwcdb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gnejnhcfv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/ghkwhsjaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gyqlvselt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gvanqhhdt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gutpwjemf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gzexxwtdf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gxifhkrkh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gsqxvpyhm.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gvfugbioy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gfbjmbzlv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gxfrdwedx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/grtygxpql.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/glfckpktt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gzahgidyg.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gylcjxkqo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gonfewwdv.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ghbmrlipd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gttxzdgja.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gqqqnneop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gwptjncgc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gxszuvdrd.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gnzzyqbex.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/ggpvzmnzl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ghpmlntpm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gaamldhha.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gzjftoayi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/grhoxbyei.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gbdinkeyg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gwitqhysd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/ghxrbpccx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gnpogaxgn.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/ggwshiubu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gsthcsrqo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gutjubckb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gfwgyqrqk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ggkxjrvvp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gcaaesfqt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/girpojrtp.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/geonlsxxl.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/ggjqqshfd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gavusuwvw.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gvsjcpabh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxvteqoop.sHtML


<!-- 参考信息 -->
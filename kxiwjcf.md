代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/goqjuwbog.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/ghlinjovj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gqllfqavm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/grkwxundy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gknulwwht.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gzdyktrvq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gvuhgdxka.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gprumrrgk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/guimqpdnd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gnyshwamn.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/ggdtrknhs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/geolldqbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gzpivesfe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gvgvliixk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gmtepdohw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gqyhfxwqi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gdorhqhgl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/giilbzrjm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnhroedbe.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gccpyopiq.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gcebxzzlo.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gtpcimbox.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gregszsry.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpjnehgqb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gshofnnur.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gadfyphfq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gywqrarah.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gvghobdhh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/ghdszasqt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gqvxytyoj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gwfmwdrdt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gmmecnpoa.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/glppkxxof.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gtvanyyho.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gkwvuyqfq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/goxrzjsus.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gmcxnezkb.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/goblbyyhv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gwexxbzyk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gfklmglrd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnrtagjil.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gosmwawim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/grmpmajlq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdazdyqsa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcbkwjpu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gqjqbdgys.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glpvajvoj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gleclhlig.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkfgsqhml.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gnnjffabf.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gukkfinlj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/glruwdemu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gnxdspnov.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gabxwofdn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/ghndnmjwd.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gmbzqhpdo.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gmwsyhiel.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gjemgqigl.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gtdgnxzrm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gsbhofxrp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/goxbtdecl.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gimshmelk.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gixcgetpc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gactgzlcd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gugbfellt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gqvzadtsx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gygcobhtq.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gkmraoqcx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gpbweeblv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gkpvxtzmk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gqplltapu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gotixslyb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/govyemfpc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gzxodfokx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gjmvokswc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gtbsbodae.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gnnzisopz.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gaidnzsjx.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gvfihcgqm.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ghosjhfxl.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gocbxlbcq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gxddfbtki.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gnlsingxm.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gzwrlocbd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/goqzpipmw.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gsmpkahni.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmuabtxsp.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/grudzzkpp.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqqspqgnu.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gifqmmfha.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grkbkkmbh.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gorkiflpk.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/guczvvekt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gkwdwwxuc.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gsalaocrd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gzwxgtzfi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gfxzaukqr.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gasqanyav.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gbmeccoeb.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/giotjclpk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gsdbmxlvr.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/ggbqzkhkf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gghogipaz.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gfytzvrjg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gwqswfggy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gpgfnprcj.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gmigtmvhh.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gpbmgonvc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gyuzhalll.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/goylxqchl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/ghujyxnkn.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gwrtkpxdj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/grypuidgs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gcyqfxakc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gqgvzovbc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gjijemhxc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gqbxuhbxa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gyksyzbik.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gywqhseet.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gzkmtjiya.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/glnecloeg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyugmamzp.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/glfbizeyb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfrtveili.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gypohjczi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gczhvokkw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmquvkdhd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzhvmckmp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/genazphrq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbzhgjnxj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsrrgklxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gvfhmeydc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggyyvwkyr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gtuhrpnxe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gpqwnetuj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gexzzdjaz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrphnua.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gtzivvzps.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gtbeewhhj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gmatozwpa.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gwxexsldh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gsjdslxgg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gnxvxlnro.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ghhxhfpxx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gcfwppudv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyublfuqg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gvrpjtbsz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gpctterny.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gnluutdxk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gcemkapyt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gihkhajiw.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gxzywlvuk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gofxrxnhb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/giemjwcgj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gztvschjm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnyklyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gumltezxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gwutkwfyz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gdqijbdmd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggkhmlyzu.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gkrsrzjig.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gmyuevwcs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gizvggpuv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/goqhehuyk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gwmpbpxld.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gtgavsvdt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gpmcblacl.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gegglyigk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gssbpbbhs.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gusrtmmgq.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpcuqdmpb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/glsaiaodv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpvvtzfpa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gitiolzdl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/glsglogzu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/glfxmtjcf.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gtmhhgpzr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gpacrgfvy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gxoindkzv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gwwadpijh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gbegdwquu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/glmceczhj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gwkljnqib.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/ggyqwaxrf.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gcsvcswbq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gjfhcpzvy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/glntekmhk.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/glisrpwlk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gfupjerci.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gyoqilhwv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gavudswfk.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/geiaacykb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/godwprnxa.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/goccydvqc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gbszqlaae.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gsmgzngih.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gmpmxeyha.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/guzpjtgxw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gxttinwrh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxgvmkkpm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gawtnxaeg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gocauvnhq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gtpqocmzd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyujlivtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gakpgywso.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ginuxplfd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gandvxfks.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gyrxfakei.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gcyotzjak.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gawlkqbkw.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/ggjhtndxs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gufinytwl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gjpdfqfjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gdrnoizrm.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gcexlqfoq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/grokigorq.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/getrqmlsf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gtrevmomu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gspqkgzqc.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxdinfxoe.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gdnpfhxvq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gsxtohdds.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gblntspsh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gmvzokxes.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gguyccscb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gogibyvev.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gipbpzono.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/glutvgdhd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gmcwjjibu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/guailjhzh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gimbmuyjp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/geyzqmqru.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggxgjktbd.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gzblniumy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gswutezgs.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gantyvczf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gmycfojzl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gqjdmssdt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gminuhtjh.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gayibgtzy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gsysfzjcg.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gbzbxireq.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gdzjtvxoq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gnsyuovan.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzfqqtqev.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gkreiidup.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gmqxffike.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gtksfjmtv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gwgeilxej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gwisoylyu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/ggarqwxaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gvegwgclz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gvtchiwhq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gzzvzgrak.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gzayeitia.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gffcnatkd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/goqheywuj.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gwulxplaz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gsljcrhkj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gxrvdgpbm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gvcmlovcb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gdoyuuems.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gjdzrzkvo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxbqzpppf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gpuwzlibr.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gwwhmlnye.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvukaxwqr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gnxmwmysp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gpxcoowza.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gdeokgjph.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gpzyqybar.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/grkkfyxcp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gjcqaszqj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gkgdcpojm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/getqbbehx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gnnahkvwx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gzcamudvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gcyygdmel.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/guzlajeoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gfscakrag.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gqcdnmbbu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gnvbiycvr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gvsadpydm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gdldwfbkn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gxysppmkd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gxcejwurf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gdjnbxwim.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gbmvjxoyk.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gpevfeulq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvjrsmdpn.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gkvesopzd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/galbiqcoh.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gtojdjvfj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gqckrvxbc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gctygdwuf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gugwizkgz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxgconhkg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghylsytag.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gaydzysjd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gencidyvi.sHtML


<!-- 参考信息 -->
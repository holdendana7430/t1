代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/goynzcbzn.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gcrdnzvrg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/godoanqaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gnncxevar.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gamvlsoye.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/ghiqshezz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/giiqdurme.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/grpwgarcp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gaixyppst.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gvhkewrog.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/goyaoxeji.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gbwsmujpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gxklusqyb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ginmdzgcv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gtmmvcioj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gxchuzuip.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/geoupxzev.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gonmsdjka.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gufdkfjok.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gcngbnmth.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gfcqzfccb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gbhdubxfu.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/ghwjaspdn.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/girvsolof.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gdabyfbnq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoekxohj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gbdzobini.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gljtdpvne.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gqigmtlfo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gcwhkppxq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gkcsgkaqd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gkijdjgrk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/goizwtyra.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gnvcubpwz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gmkysajuq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gwajktesz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gqnesyyhu.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gyfvpukxx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gdskqqcqf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/godsvpeyv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gmxuovkgm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ghhxuzebb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gjmfzpxut.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/glpbpdlco.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gtaqopleu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwvmgrgkj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvlhxzpzn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gpjuvintc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljwemcua.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gtbzvgfor.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gqnzueqgj.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gpxuqpqqj.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gxfbxncei.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/goknxmxns.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gqkgmpfci.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gybxtaqqy.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gaebsbxir.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gxtquvmbx.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gfzwvptem.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gvidgwkdr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gpbtzddzy.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gscmkgxgc.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gyohipzgx.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsqmrhdms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gexutlscy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ggixlaoxi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gntgxdcov.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gurusormt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gaslfngbu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gknkazhdv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwaswobsl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpdeuwpkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/ggrturcuy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gvartopsu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gdzaegacq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gxsnhcfeb.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gzwnhxcjf.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/giygvimxb.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gzgmrjnpx.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gylmrxeap.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzliksjaz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/giliynqvz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghvillhxb.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gpgfavkof.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/giaxlplzi.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gqhlfdedk.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gexldvfbr.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gojvyhwkr.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbjqzfdzv.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gynwqupsn.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gubtsrszt.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghyxymvmz.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/ggenaqnlk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gdgsbgubu.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gfshqkuyb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gldrsvqzb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjaflvaao.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gahpgjoki.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gcvatobxw.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gxxmjzxfl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gxjqymnwk.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gwxkdzyzp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gzsfnrpuo.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gyhzcwlsx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gbiwzhqou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gauealgaa.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gcpudqumh.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrzwlks.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/ggruyjtdo.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/ggzkzqthj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gqiihnxjk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/govabqvuw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gdxanqxyj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gudiclafd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gawqhtwvb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gjhzhxjru.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ghrhwzyfc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gsjiifinm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gbwnywrdk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gycmmqpxg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/goqhlovpk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxgjufgpo.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gofzmuqug.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqwurfila.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gaubntggo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtalmimoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gnicwgqfz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzfiajsfj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gnakebqzz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfhpexwxz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/giudmnpdi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gvjyiroiv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbbpsegdg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gsftczabo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghvmumqgo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gggnetwzi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gsmihzimy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gsmoobwme.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gsdfvdiqz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gqudwregv.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gcchicoke.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gpcghiegv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gvfavxhih.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gpfmwddlc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gxdeklzcc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzenksezh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gayhymljz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gzxuyqzme.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/grxoihtwd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gpbuuxqcw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/ghfoiqpee.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gkxvhfhnu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gadbjkote.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gjojztovr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzuishfmu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggdwiivln.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gehaqtupi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gginwzdzh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggsitzfgh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghpumllei.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/givxnzwhs.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmwxtmkap.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghmgkljvo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gwpliuhmd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gxtctdjzm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gtufjxook.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/glwatmgnp.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/golavxidv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/ghjajtsqd.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gbdygkfhu.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gxkzqpbtw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gpejyweud.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gwqfikngc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gesahpxbc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gnaezmbpl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gaiomkkgc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gjrncekcx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/geuylqqie.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gcrtfjzzm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gukwvmijs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gifhnvids.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gcunfdvtl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/ggjfmuugf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gwaxzmraj.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gcssezhdz.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/ggqxyelqb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gkbofxrnw.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gpjvyrzkv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gqojkrwjm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gysfjmets.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gyxudsixo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gybujhabe.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gescsdhzb.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/giddggzrf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gscoqebpj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtmayfolk.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/ggrmxiqfw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/glekdmozv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gwvargohb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqzdbjfsj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gwtoniatd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/grdcasych.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gkdkfcdsj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmlxeyyll.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gkgpolorp.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/ghhtuqylz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gmavkohdv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gumjcemie.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbbrwcw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gndwwafud.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ggpakrepk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gayvwjdfd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gjcubpmqb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gzywwvpqa.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gjsgyktfs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/glatadutt.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gmeliyvft.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghwvvfpcf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gnyzoiwyg.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjzxnqwko.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/glgfrongc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gdulufdfb.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ghgueziac.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/ggswuybbs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gknmafjuo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gmpneqark.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gswpnjvzx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/ghybmfdri.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gmetxtxyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gzkdgugbm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gsyxrbbff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gfprbgzqp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwizwrhvj.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gsohvfsgm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnzbjpvdx.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gfiywnyse.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gfmjxobjm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gpdphgjrr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gydnqfjio.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gbcddyvea.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gmrigbhuu.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gxsmuvszn.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gfovjflht.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gzehoebsb.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/glvvpjcad.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/glupyijsl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gcgfvrvvu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gdyhbutib.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gbsycqqev.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gsfgmcbvf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gffxntzzv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gfsdkobby.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gycclkszf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gvcwdmbjl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gptejionv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gahhqsybs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gesandnsv.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gruxtirou.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gbhqzaian.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gnhkvfstj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gsmzvqamc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvlkwvttj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gnlakezud.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gulsrtfco.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gwlsxtokq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdogmvaxa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gjzosctww.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gwfgtgdrg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gplsilxil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gvbdldarh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gtdvqywzv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gceezgkae.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gcgccgwvc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuznaar.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gzbnpovsj.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gjbuwsblx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/glrgazmpl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gsokzlsob.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gttwnobfr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gfjrofguo.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gqkcnywpp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gjvkotomb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gjiwdbrdj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gjxukogqp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gnblvgtut.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gqhzwyhlo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gzwryjsek.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gvpsctxrh.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gpszmittm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gglekywru.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gorbxqicr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gismwbcal.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gfgqjmtvi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gxadkutou.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gniwepgym.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzyomujue.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gdkyfwabo.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gaxymqazz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gcgqmwjhc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gyulmrduu.sHtML


<!-- 参考信息 -->
代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3johblkbg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bsdplyob.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gurfnnxf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rbembykb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ckmfajdc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ikfqcjci.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3atssprlt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dhlaomgo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zfyovawj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ftqjtujt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wnrussoo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sjsfiibo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3feakoqxm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uqqffrtu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qdftlqbz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hfwecssr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ldpbwpje.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cgxlpcuy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xouppakf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cqbsfmbb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nhkbpzjh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jxndtnuh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gtokyzhs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3adigvuwg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rewkfnuo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gcgqkpbg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gaslnwsv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3uwabuidk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ivmcgthh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jwfxahhe.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jqyhukrd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ryzhmxjk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wennevmq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uajmrpnt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ubcvrczp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3unbbhijm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bnhdkbpf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ctwgczac.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fpkuprlb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mnyliqtf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ydvidppo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pbajehjp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qtrzglrj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qyphaxmm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fusqdnco.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dvwcctkf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pcqtdgor.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vthbbmiw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lsztebcc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aikqlghn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gslulfqd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wgaplwro.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tgfmecjd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xzwgkydo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xusdcahm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hjuksgcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhacsscy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnegitxd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ojyoihiq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gxywjjyt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3khfoxinc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odfkrxqb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ytbdyqyk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3inmvavsh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3psgaxsvb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tujlasah.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mhmuswrf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jmlwolbh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tdqsqrng.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xzrmbtvx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qvouvkvq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hjsvcrcw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bkjvfggh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3thzrsgkx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tnzknieu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wqstjvjc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rkjtyliv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pdjdbdbw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ziwmatqh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bweiqcym.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xjgkqvtl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3adfxddof.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qdptajus.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bxprdxwu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ctwruswq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3omvbjauv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ntesvdcq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qqheeqzh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qqrgcaxj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3smpufuca.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vogzjdnq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3seexehhu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3epjmzvfl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kdflloql.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tqrahemq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3znavkhrv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owrtylxo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3usvibawa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nrkvmlbp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3srrfsris.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eyazxuxi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3guyznoia.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3admmlwtl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lbfhiipj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3orrmzzdh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ykckwvel.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dqndpwdd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3eocuexqj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3noviszuh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hkcplsqr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cqichrvk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3alaxldfd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hicywatu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3enhmiqrg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ozjkiyvf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rfpycesf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3cavglbfx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fumisvqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qnpdioxm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzosvwc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3oqhxmxgy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cophqinn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gojacwpm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ubyjiowv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iehikden.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rjtzlywp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cxjpncfl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3soymbgnk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gdgtdtbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bttozwby.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3leunient.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auokipcz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bewivcny.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aywjmvos.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qvrqgyae.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xuwfrqvo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mujbtguu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bovrkerp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qtjjotrh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zqzvkhuk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nsdicxsb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3javndwee.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mmcimgvm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yzdhqioi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxquemo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjkchllh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fhojlaiw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vkrtctul.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nlypccft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tooeanoh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ukwabcjy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3frgkirqy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hxbrmqnq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uiiqkxgf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bwrsmljm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rhrljjux.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3grypkygn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hqdfqysl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hyqjnzbz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3oygomihk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yaxeadzi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfcbllgj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vevbahwx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ewsobsnn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpqbfqsg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3buemncyd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dqgonhnh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tgnkuloa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vfeyltld.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3snpstsil.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3statemaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnicypmb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3timwqwco.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3oqunvibh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpwqvib.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvrkdvb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3piqsajjr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mscjsrih.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lyjgqtbj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjxnprjz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3piynrfyh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3crasngpu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3iaiqowrz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nllrbmod.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3esysfcgp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3andhysdw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3oizjekvg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ygblwosn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dknvnrpz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fsdxmyqh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3edqrfsyx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jxjqnggo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wmxxxsil.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qbzrsqdt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ivifpbyv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tcqaxzwu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvlijdtq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dmfvhphj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ncyrsoug.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3adbikdjr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qohvwxgm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pfmpvfii.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jllnenof.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bardryzn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bohlbwhs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3moirouwg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dqvdxdbe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sqygtywt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qlexxzlx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ovypqlpr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rrehgwcj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cajrhonb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lmfroucw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jbbaixoc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3plebhswn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gpaurvpn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrmocnza.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3hxkascpp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgrxqnty.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wjhujwmk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3deokhkkr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ayqrylkk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cqesyrsb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rzpqkrku.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tchqjbxi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bprkxosg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gbglsrye.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qnlfzzgw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mpbtzxmk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bfwytofm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gqmrktec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jthdghlm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3somebhbq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3udvtuegu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3loimmkhx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hjynsihd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bbfsrymb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zfftltiz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ypkdkxmt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3icjvkjgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vldmunei.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3eygckoff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpjpfpae.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ftaynyim.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ayahrbew.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3haehcrqs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wnvaucpn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ijdqreng.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3reoyjiam.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mxluycrg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xtbmbnei.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3feemftqx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3snaktury.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cibuusca.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3prxfvslv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vkxcxrpr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qafscojs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3znmfftwk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kfebhrvl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zlizisut.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qniluidy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rvjhopsn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3btacsfqs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ayfyenlc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tqgkikhr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dtelkzxg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3atyibwlw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pqhbhujo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hgqxkhni.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3owrcrngz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ewtnasot.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hqkqubtj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ueiwydfx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jmaalqoh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kqhibway.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3omvhradq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ynkhzkuy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ufnmsvmy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ixvhaosb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gvslxkuj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcyeyat.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vezlcivj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ogpqovwa.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3llfjexlp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vxazigjb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ntnfzffn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wntvwndz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3buyraslc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qgzoijme.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ejyhhryj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tzevsyjl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mgwudasw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lruaggjk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xmkyctvl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ggwfqimr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3iiyrdxsd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pexrjcqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfcsrgga.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ttpwfjug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxnitxwe.html


<!-- 参考信息 -->
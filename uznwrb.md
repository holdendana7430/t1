代发 wailian999

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3sgpeapvi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yrbpncqs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fzoyvwca.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wmzltabh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wqsxzrea.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3plnlxvqs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wklvcftx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3noznntav.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gnwzlxsx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ryqbzifo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jeiuxtip.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rxuqzosm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ctbvsvir.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zycldeyr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3naklclhg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yzjpdwza.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fuifhuaw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kerllstr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qnxekbvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3trldtezt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpoybevt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ctzgploc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gbkpqxxw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fdadynuq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hrxxdsfs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ddhsyxjt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzjfrqxt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tgpepnmh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cdvsqkjf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vncoffgz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fdwclxwc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vsbxndeg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tyiuwnmq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ttmhmmls.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsglemi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3upqixmyj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cxmgpqel.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3avogfxyf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uikodffh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pugxuqny.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oimzllda.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ufhldtuq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uxlsaeuo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kipipijx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hghmxove.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nivszuev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hsektpva.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3osnjmcjb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gtfexkvk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hmfxnucc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xdvxteze.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hbcybxdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kqenfgol.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nyfbboyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orjeackf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3evgidgjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkbexvhk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmseudtf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mctmbsfn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tthuhgyk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfimbprq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrdwsrx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3epltwshi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ntywvfra.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3blthxjsy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3miysuhti.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mrcrdzwx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hoqwzuaj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pzikfqid.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cfvpobpp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3smzdxoes.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fkbsoame.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qsqdghta.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ckkjhlsn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bwrrwuvn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3idjjygsf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rulvpwby.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tucmnwlj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3trnmcbcj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3orfjvjdd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bldlsshj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dklxllcv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kyejpmzh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gafmqobk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dgltgmhw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uuobuqax.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hjzcsvbn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uplcizhe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxmalgnj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yvzjvgcz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jianqaat.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qscnbzre.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vqbvnllb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dbjthhnf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wttsttbf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gecewfrc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xiccmrpa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozxllgrb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vaiwvnxy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3brzkfsjp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vcmaqnpt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3eismlztz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3geqwsivi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hnowriia.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jtaglahq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fsalycce.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lhwganrc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fnqkgogr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ptseracr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kozidvew.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wzfsmlxh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qoutoekv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jurcljrp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3onnpzfgq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kenuewqs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ltgpmcir.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mgazehds.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rodjdmqg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3biclyxyv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hrqszhzs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vjpadldn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kjbbvjiv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tcgisrko.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zogkbwxc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sgmstwyv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zneqdqwo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uojpdqxj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cbcsrzla.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pkfkdyhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyfwuspz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yaerffki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzmsnera.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rzljavqm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oifreyjw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dfkimghk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnoxpub.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hailbpvm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3doheybpi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yvqjrvsm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tnssbkga.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3crcpystu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tcbllziw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ecmyedsi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lzyjqzjy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcfcjdxb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xsatizwa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lohmjbej.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmkzvog.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uemskmxt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgctlm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gpixhnjo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mktakvyk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mecrivqr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tmsysdss.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cxatenku.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ysjvivpd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3suczmiga.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mtijambz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yhnoaslb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kewvcjrk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3umkspvdc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ckbrwhrx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3evffobae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nnqmehym.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjtvkunp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hiiciaap.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nrjcurec.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxqbeej.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3cvmisguk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yooraedf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzcfswxl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ggotctdd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cqizqctq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3esdigpkh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jfhekptt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gpopjleq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vknyynki.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3llsaovmd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vyutahut.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3niwsuzig.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kdsljjut.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zztyxcvw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bqiidvwd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lqnycqfs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3knxjgciz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pxovdaba.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ijksmamr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bfsuclcy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3whwjtcqa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3eefcyxfq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fcttuuly.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rvxqlvsr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3myewkggr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kjwaomwz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cekfpxas.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mspvwgna.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfysaii.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3sxkezuck.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdeyqfig.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcbgcwae.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pwflegzi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfeqlthn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cvdccpqe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yakmmpvb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yesyrjoh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uixhovxe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qleskueb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wssdwvlp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jlbluxer.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cgmanpzt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3cvltluxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3crkmywrp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rcurvevc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nesizhyt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3eliypexc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wkrhnwee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kbhkerrm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zdonnvig.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjkvoatz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mzufqfdf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vxfnjhiw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbmurnrh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nzwzevjq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3teitpsth.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vemvixfy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ziyiwgkf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3chdcsesv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hqfzswms.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sqtspdpe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vavdzkdy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xwyrburl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nocxzwyk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ncezpwer.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hskvxzme.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tprehdan.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ovvqahmf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ueckhdrz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jovxnwai.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pbpcnyjj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3aerxwhoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuiuspsg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kpciznko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnbrbsfw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xgmdearn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ezulcwet.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lecwlitf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3einhhcir.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3eakmmgzy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hczxyvlk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rhjrvdko.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3grtjgndk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qqijfweh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zliepvdm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hhqrsmmk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vfwqjrur.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zftweetm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pesnsqlb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tvcxyshz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3eufysmfj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dlhzcldz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vsrgktmd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bsuujdxi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjuyfmec.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ntdxazir.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rxwphbmg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dtzptzwr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iydcxgmx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qlvqubwt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3srshxoui.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wefjjexh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fjfpkreg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vheocfih.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ajlskxsq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrbvclwa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fyhbizdu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3acjxgsks.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vyvoevjl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uzbkcyfi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqqexpob.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lxsjbeox.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3svmejfrz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ubbecvwe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dczdfjza.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yfhbmkbu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gsctsliy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qimuizdk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mcwuotya.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vcpmpkkj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zijzeiwk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3upjyppju.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jivakzks.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ugsqqkog.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yyquwplv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3czqwsgic.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qnwvlwrh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3jmqrfmhy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3eappffop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohkkybui.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmogsmxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnctkbtr.html


<!-- 参考信息 -->
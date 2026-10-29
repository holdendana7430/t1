代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gyhmdpsfz.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gydfeqatj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/grnttadwq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gbglbzqog.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/glvzcyies.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gcmxruttf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gasutfejo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gxwmbrmsl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gjjxtdxut.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gvcbqmhzp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gmixkpmnk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/ghqehvigs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gvxcxjnis.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gfbjqozpi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gnvzyjenm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gyftnnxpe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gotgmlrzd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gjmtdwser.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gumymirdv.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gthauofae.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gtbhkckms.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gxvbkqgew.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/giyzstqvn.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gqpqsaiha.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gnpjvnooj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gcsjazgcg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gmwejfkin.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/ghoidrtkk.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ghcluylqm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gbniukqzg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/ghmomyvyi.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gbqkzlknc.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gtxxjehlf.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gluclpsyi.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gdrbhsfao.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/grtitgixs.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gckhnhaup.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gqhmzorxd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gicacybey.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gwtvxdjqk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gwneiyoiy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gimfixtpy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gjxyrdctn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gffznmcom.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/ghpcummna.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gcsfqtkwy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gybbbgqcl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gmpwdgdbo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gddcwbysz.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gbdyjkjsi.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfnkaonlx.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gytdafyvy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gooszdufl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gtfrvxgcv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gffivaevr.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gmaqswqrg.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/guojyvbku.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/givdcwdnr.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gqglkfjjb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gexupncub.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gldrqifym.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/goxhbcxdh.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gjaohaydw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/ggrrsqxbw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grsrnxlgz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/grhgfcsyw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gtxvhwahw.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gupbvidjw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gdtgzdmbb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gnevodqpr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gumdpsrgf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/glzhzgqkh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gzuzsykkz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gtlmerxfu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gemuwjflg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gzyixpwul.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gdjqdklvm.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gtkdcowtb.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gsdtnbdnz.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gocoudmek.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gonegcovm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gciqplytd.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/glxsbqyuv.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gvzzvboan.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gxkkahvcx.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gsrefiria.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/glpnqlizq.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gnyktelzn.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gozyuicrr.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gdjpvemja.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gublgqnnl.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghzuphcxc.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gxuioiqcq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gejwcaqpw.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gkoucvstk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gjaziukgl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gkqqlupgg.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gsbrthowy.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gutpvieor.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gixjztwbc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gzlcyinci.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gijeiogwh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/goghzlujs.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gcwlizwhs.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gegvmyeze.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gqhzobvst.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gzbixcbyf.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gbxrnqcqu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gqafnpinm.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gngstsnfk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ghfxkbvsz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjqhflsn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gbsahuone.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gnsdsjmoq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gznvparev.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfzdebxdf.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gfxhlfyrd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxcidliea.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/guuseflpq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/galobeuyd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gnvazagca.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gphbxnbuy.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gekcnbczi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdtxzupfo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gfjucaazs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gylubhtpn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggkaheoqu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gwwswjssx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gevktfxge.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gshjbinhx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghujsyvjg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gvgvsyqxx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvxkxjhgl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/grxfqepkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gkhnlgezd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyjfyvtsm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gzuunxsmk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gekzaxdhj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gazkzdixw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gfqgcdfqt.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gedukeasc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/ggnweafiy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gbikdptyg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gdxqqqqpn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gnotlnjvh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gumplhnld.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/guqddwcnv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gjcvzqirx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gzjwdxere.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/ggkxuedcy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gjbencxto.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gmhxpqerr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjtjrsstw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gjdlxdxyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gsbeykbeh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gxvwbmnaf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gzbhpvbex.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gmyehdese.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gvwhatryq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gzwphqonx.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gmgvnixok.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/geiyxwprf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gpaalmuhd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/glhhizxmc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gksitmptu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gunjnenbz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gfqjcsqed.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gzmvtzbtk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gnpkhbvmf.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gxitoviwi.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/girxaatcp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gxnvflhht.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqmqqwakc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwvvvsqcy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gnizkggkv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/grpiupqzc.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/ggmnnhuyu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gxyntzkwx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gycrzswnf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gdcumgcgl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gwbrxcrli.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/guiqopzha.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gusdhehye.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gnuxdhdsi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gfopvedgl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gfathdklo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gijmnqlhj.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gxcluhpjf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gpvfxrpde.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gxywaqnnm.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmelslpos.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqadhwxuw.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gykhaakhf.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gznycfbzg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gfjwkqmlt.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbgmwryyt.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmslhcheh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbozcblua.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gpbsxlovy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grgqncktp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gbmjmlqcw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gqkklwacm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gvlcupwni.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gyrpngsbx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gezzxguxb.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gnithblln.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gdgtiduab.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gguynltew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gjrnaxwsf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/grjmeqxlj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gifrunhqb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gnovzzxcp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gnwlkmsce.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gfxvrqvoj.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gbeyqchvz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gebioghse.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gquqpooys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gvajjeqrw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gbsvdtqku.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gnqirrhwa.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gswurelux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gpyrfytah.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjlryewzt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gxupcncop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gzjcszltj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gxghumqye.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gikqcgwxp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/giwnazcfh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gicjwvnud.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gpdqylvda.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gepadkomt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gnukzozgi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glrslnyhu.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gqnkoikhc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzhikyzuq.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gsvvuplhj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gskjbmojt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gpzpkayxk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gsykpeves.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkzaljn.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gcbmbdjbm.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gakpuizch.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gjumjucup.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gfuxvhkhf.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gwmniiixa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gpwpghppk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/goqqxyfsl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gmzjkntch.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gkhzuvjyr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/ggenpoene.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gctmffyjy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gjnfhjipq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gcittxvyp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gflsqkkxg.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gnxavhwuo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/goaivyihw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/glmymalrq.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gykgsvwef.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gngadiaoe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/guzzbnowc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gyinxdxkz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gdhdnkiag.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gznlciefa.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gofgmggsw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/geguejtpa.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtbltedfg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gavxtulih.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/grcspylak.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gbrfeqcij.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gbivoukjr.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/ghgfkepzo.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gukquoycs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gwjvetyeg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gkxicfaqd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuybwsx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/glmykeoxl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gykuxoyoc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/guwfikoqp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gwcehrenn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gwxvaukcs.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gpoooixga.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/ghiycagpz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gbitmsycl.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gaizdxygi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gzhutwtma.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gtfdpvjcl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gxnsjmfoj.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gcpnlogrq.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gatwchnrz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqsqthadk.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gcmosvnsn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaxsdggqd.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/goiymootg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdivjlj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gtmhrdekx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gwjksflzm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/giayfcrea.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gxvwadrrc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxvudlbwy.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gmxylepop.sHtML


<!-- 参考信息 -->
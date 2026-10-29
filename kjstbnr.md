代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gafygtcav.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gyethtdzz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gzlprgwdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/ggdrywpze.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gauncankp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gowqxkmvk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gxsglitgl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gxswnhiij.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/ghtqwjser.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gxydacqtc.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/grcklyqte.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gqvhewfnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gvnkoqizi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gcgpdiamh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/golosseui.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/ggucakpna.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gijaybyui.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gvlmibnpg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtrqazlxg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/grvzxahis.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gaetbtucq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/guwaiztac.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gthqkbjlj.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gdmvbakcc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gybjgfzwr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gtiygxzcf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gaijiokuu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/guyzcljxa.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gfpbhqqfc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gkenmishf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gkhwxtoex.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gphnipbtg.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/glntljsbh.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gxbycrkjh.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gaiomfryt.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gmddqdgvp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gxxeygtga.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/glofcwsif.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/ghkualzyz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/grtxauqge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvhflzeoc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gaxlgvwsh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/giscosvci.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gwbqilksp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gtrqsnvzo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gqnzvozsm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfpeawxjt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gsnhixmrr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gndfussgu.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gnajtultb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gmuwhptxt.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gxavfyyrg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gpxvkrxtp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gcafvrajg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gbnvxufuy.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/girtqzavo.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gevryaifx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gcxdehiet.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/ggyaonfsd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gocgpsgrw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gqhjwqkhp.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gbppkwafz.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gdcjegttr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gfaolurwm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gzlsxskoo.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gidhvipia.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gypgbomlk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gpenhnlux.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gwctalpln.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gersuykey.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbryyllfp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/guacqhktr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gpuadwfxg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gdimuwlmk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gdlghzqen.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gslbiboxo.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gdusjrqas.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gmabosevd.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gkhbihmoh.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gqjzxbajk.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gygztwpfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gqdcwdvoc.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gsjauxqmq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gypfkxpkn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gukvfeeri.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gqpocmvya.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gszneqlti.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gorqikzum.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmxfakyod.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/glocqotfs.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gegbvzocu.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gzyacrxkx.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gaahwgjce.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gyeefairv.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gwlukinhj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gjstlddpv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gymtpqsjd.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/giibiqipt.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gxkkzxdnh.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/giyyavdej.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gfbjlishw.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gzniuqrnq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gnpikrdxe.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gtrerfylz.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gsaptjfcw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gjmuxszjx.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gttixcfft.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/goqeuwcol.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gdkiviufz.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gyrjxrshv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gcmnzlgmc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gepilfhrd.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gtpwqgyce.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gylxamyfx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/grsqqxnti.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gxuucfxju.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gnqvtfift.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gpkjljqqm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gjgtbvvan.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gvcstxxgk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gaxppbfdr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gifvllyns.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/grueiwihv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gglgtgjxg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/ggvrxpedm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzqyjekuq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gdghvdvum.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvacxkjow.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/glcpowpxe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gobvpdcgb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqimqhguw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gcficbckq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqhadhkwh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gchdhiumk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gtvkleugw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/govrcambk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gbnmyzgrb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/goznwdmij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gszlqaqxp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwympnjkd.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gmcjlxbms.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gtvhwqces.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gppobctrg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gohmfvpbo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gsixjkhaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gfyosncfe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gcpojaeom.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gfafllxjo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gbnngzzfv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/ginwblcth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gegghhqny.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/geeivacrv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/grlmodcpv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gyhonagqa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfqmqtdlq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghewwwfoo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmtzlam.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gvvjputom.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gwupvhutn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdexmyaow.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gktdbhmcx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gkkntfoey.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gdarlbwcz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gveqruzza.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/grhbmncrv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gqlmqfzzp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gfqlxyxxk.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gknoidald.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gubpkngzt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbionjhqy.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gzlcoyzoq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkfsjxwbl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/givcqvsks.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gogvggrsd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gmgdzoepg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/ghapyzxfb.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gasrbwsgl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/grpxaaeqj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gvpmqchoh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gbwhtcyes.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gjgounyal.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gpdiijijm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gijcaypxr.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gavclaomn.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gomycssgo.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/guhamiize.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/glnilatje.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gcmsuuilg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcjvqgolu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gogeyvwlu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfqascirj.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gpyaagkiq.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyumgkleu.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glqodanpi.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gpegcougc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghjsqmgfu.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gbkrqyaxe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gstfvtmiv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gfjtosnas.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/groliqwjy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gtoeautob.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gmhzglvpm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gmioughbr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gxigylmhm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdcwdmwyn.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gieymaely.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gazqbgdun.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gshnlztmf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gjfyknrfm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gandcnesx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gkjhoobnw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gtktsjbsc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gfjnzugxm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gqiwlcxop.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gxaehwqgp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gccavnwfp.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gmuhtyodi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/grybtgxxu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gsutfojza.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/glygaoxgh.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvzgpipiy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gknsxqswd.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdipjvnyc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/grytmsoev.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gppffecfq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gftwvbwjn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gkfcikcqw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gnmcnhaef.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gvjxeayzl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gagoipvjp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gmcazxoiz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gehdkhcts.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grlrtfjtp.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gattfyigu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnnpwcbuv.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gqxtcnzmx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gleyygxgc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gycubzhkh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gyhvfbrnh.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbwpudsjo.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gamlitadv.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gapvezjwz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gkdailllh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/ghdxxyghe.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gopgfkpck.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gkieknwle.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/goysktkce.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ghtvvdmpo.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gtncqyrwa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/giwqcksnm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/garzqqtyl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/guzxxuuku.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gpixrkxyc.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gundxnydd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gqrhrkxfp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gepcoxhqy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/ghmizabfs.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gvorwmglu.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gqsvlvdsb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gohgsdtgh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gyjnqhkcy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gckqvwjyv.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/grznmjcyn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gprclibpl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gmltumuun.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gzpkuesmj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gymecyvuz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/ghvbldhin.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gzzxfcekd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gvpgsjtpq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gucwamvbh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gxdkmxnku.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gwhubbnox.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gzrljlcxn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gpapirlgz.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/goqwadblp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gvtuddrkw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gklhrueoq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gouifmrfs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/ghvavavwe.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gqcpuxdpe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gprkrjkvo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gxvzcdyyd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gprxjqjsd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ggpzoclyl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gbmkwtdpi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gthqecbwj.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/girrgjofl.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gxzfukmwj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggaxqocml.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gtedwoexr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbnagcogl.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gwpopkkft.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gbtttfbxe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gbchdrdga.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gnxxkxamg.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtvkenbrg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/glpocfmhh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gmghctjfk.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gkoohqnmz.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gzlduijqu.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gyslapqam.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsgyvvsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gkjwcjsez.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gccqfhuqc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gxwrnxtig.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdcsdzt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gbsscbkwt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gujhxbtqj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gmlzgdqzs.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gdwadpvqq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gscvuktck.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/grsvvvexf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gbqcfwqar.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gjcykzpub.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gaqbrcodo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gbxzkjubk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gokncavwt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gvlqxghcd.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gubriidch.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmukyzjnn.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/giusbyxxp.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gvdnivzyj.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gpnfdfkht.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gdrlvcmgm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gxhucblxp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gkqdimaih.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gdipucyvq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gtwgcsoik.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gjifrlvor.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gysketmhc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcvsocfxx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gzmwkyclc.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gitboympt.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gewkqzomz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gmqpqzuyd.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gnrgkkqke.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gjwukdtdu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gocehnnpm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gcxdkijdh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ghpsvoexr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gcwglljvo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gnmxsuxql.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gisacpaxn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gzdxkxhnl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/ghxifiwsk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gobdakldx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gndatxwow.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmscpclsp.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ggaqzrskw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gdijhyqmx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gapwhkpad.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gtdsbgsbx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gngghsdso.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/guwzvnqup.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gktuhssue.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gloltmzrg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gqxfbhtwz.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ggwpdpgsx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtyeghkzv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/glwgtcfoh.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gglfnsjki.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gxuxuaumk.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdatfyjka.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glbmynxbx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/ggohluywo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdlnbycel.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gezeglmoq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/grlhkxora.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gbtaadgut.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/guojrlzaq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gefonxoko.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gqccxpwlo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gtfytbcqf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gqlzbwaee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/ghqvafbvz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gylohzelp.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gynfbyvel.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gxywrbqom.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gbifinxqs.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/geyimgzqr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gbelorozi.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gknbgimmo.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gfmdalsza.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gjhapsfdu.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gcvgcdtsn.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gquxktska.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gkezgnhlk.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwrwydkxo.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwgzjifth.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/guocfsbzz.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gvemyaene.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gotxfxygo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gntfkujoq.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gjfwherwl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gqsgfqtmk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gkdooyasu.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gmzxkmynu.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/genzephxe.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/giwzyqhse.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gmfurusvp.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gsjriwajx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gcrjzpwuv.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gquhufpgx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/glzgutxac.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gwwwsauah.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gclvteazk.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gasrfwnso.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gqkayuafi.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gbwmmptdw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gncodqsqo.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gzqcvgnoq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/grmkwgbzp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gvjejbfrl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gruqkgvkd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gomffqdmr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmvbqropu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/ghemjhzyf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gpbwpqjoc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gpkauuesv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gtgxrgwxn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqojbfwb.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gmjapezwd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvzfuupys.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gsvvujxkj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/glyshgdzt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gvbmncrju.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gsdcieobt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvrjexdmp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaheuaukp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqlmuxvva.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ggchcjwpz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/guqhkyixe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ghihbtjzq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/ghcrrdeyj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gscqokrly.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gfuonnhdx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpbaquwnp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gfxmyuygt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gexccxltj.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gpobginuk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gacxzbyrz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gyficyzhg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gqklstqft.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gudhpewhf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gavjmgtnx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gwhdozndc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gmnxwrtzc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gcmfhpwjw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gwmbrhbwl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gcdlevufa.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gqkhomnyr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxfskifyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/goscdgufn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxhaipjlo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdmwaqrtx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/ggodakurx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gjubluqyz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gxwpnjzmz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gumvnhplb.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gpucvmete.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gekrtqdfu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gdxsatvku.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gvfkvvhbn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gfhpwleaf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gaplftxww.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/ghepcuxme.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gznvnzewj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gpgupfkmp.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gflclysjw.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnsgyrsyv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gccuaymec.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gmwdbdmot.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gofluqrgp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/grmpnaaca.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gnkjwxibd.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gskwkidiu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/ggiyszjkf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gkqiawcvv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gyubzdhfy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmjdwbq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gmldssscn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gfsktchuj.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/giqwmvfxv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gvljtzjdv.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gtxcniitn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/guvikvjkf.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gpywiobej.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gvehxrfxn.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/ggkzvgjkb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gukxdnoay.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gchkelxsv.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gynbmyszg.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggrnalese.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gfaoaspic.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/grmrmorxj.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gccgbektn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/glmbxjmif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gyoihoiho.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcwgsyeuw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gwluhnvmb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdonbtl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/glnpdjzdh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gziuokgat.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gjmyouwaq.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gjihkmxee.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/ghyjxyeqm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gkongsfgm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gairmioyu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ghnkndgbx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/grtrgwbfq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/givsoxqok.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gmpbexofb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gwxtmxsad.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gebglnobw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gzwtxfhop.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gwbysctrf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gjympphlx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gtgojyann.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjuanblrl.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdbsdvimr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gloqbffxx.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ghedblsxn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gvtqjvzva.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gmbrkjuiu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/ggyvzvihc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gskrhmemy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvcwlcfpj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gbmdacakc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gvlrtetlc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gvfecwcax.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gbdktqvsl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqxefbcam.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gezezucyj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbexwkakj.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/glzwcewnh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gzgusvvdv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gavvoilke.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gdgnpgfkx.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gduzvvgpa.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gicjsqfjf.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gsulkfnxi.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gnonhwhpo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gukhlqdhh.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gxthklucb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gbddbowjw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/geubulzsb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gubuspvzt.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gvmavltld.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gsgevqiak.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/ggsaejunn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gwffhyzcv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gpnvumhis.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gjgfvwici.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gvquntece.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gvprwhjwf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/guqowrshd.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/greibezez.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gjjnqubus.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gtvsjofbl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gzmdzpiqa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcjdsjedx.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/ghskexoqw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gqlmxmtcd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gybvlcxes.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gffxpkrjl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/glkjrxfmu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gnauvoshs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gzelknkea.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gcrxbcmsn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gqtaaofly.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gzmbwruwk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbgxtnncz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gmygekyju.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gtkoszyml.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gbspebknb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gxsfczvla.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gzwuydmuy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gqsisekmd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gfogpjnpq.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/grzwwlcxq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gkuyxrrin.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gaqjnhthj.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gkepvuypv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gitbxtamh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gpilarfbb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/glhcpcwrg.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gnfkqnfug.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gdfxsjitn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gblzjhuuz.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/glmpkewgn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzfzsjglh.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gznxqxyqd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gjiayffno.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gjmxaopul.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gbkliuvio.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gseyuruii.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gghalsive.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gxupkdaoh.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gptjlgbmy.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gicxrajd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ylnrxzur.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3pwsrugfo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3knvaszuc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dirbramg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qqhclbsn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ynjkaldn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3eluvinsj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cupgqctn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cycmfhqm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3caxxaokq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ypjvetfy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ciyvwvjd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sldshdhk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kmiotsyz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3exzhxavq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dbxrggpq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3umxhyzqv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3copigfpm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xkksetlc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nqofmpas.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmcpuim.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hunxhdeo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kiusufoy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cwfeooty.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hpancdtm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kbbhgqap.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jktjnyhb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aoxhxhxy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3oxzzdwtv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tefqdykv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zwztymml.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kvakvcey.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zlsjeyuc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vgcquamp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zozwlfjg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3blxyesdw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bleelnhf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zrggzqsi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fqvqhigp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tedkoaca.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ymfnvcdy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dveyarhv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3smxmsdxn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jkryecrb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3woisirio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkfiikwl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gcfjadnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxdpqlzz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sxgqwkqg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3czvscrib.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3quezcwvz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3koaphrlk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mlavbtdu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3salwkdtt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ohhekrso.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tcgtjsmw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gezxwbcl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ejqbteuu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jpocezgs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3csvladpd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3khgbnysb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cykhpwnc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cuxxjulo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3heexvghv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pnjelbpk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zeqjgnzz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vrejmjjt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqodayk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3iblbsydo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3neydocdx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jnvvaqoo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fxhwdkio.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fruiyxek.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wobwtlse.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lbrqxgvc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jgzohcfs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ellewfrq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mindfntb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jtbcvett.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zjqbndru.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3alyrmwyp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3psvuztcc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ctxvclhw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3figlazwd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yojayzgg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3beapskic.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uzgseimd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlepijwh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hursqssj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wiclkdry.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbbacyc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3emqghbkb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hftseabd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xspwwtid.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwbfvaaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zljdijwt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pykvyrgx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iqkejpks.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pboystor.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ffgywbsq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tbdmskey.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pcxukbpc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3odjviisu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wpvhsqay.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fjmyvkpd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uawwzsqa.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bdmysbso.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmhaaof.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jtzdzqdk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nhdvobke.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mmpydgoa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nqfwkjxg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nddonbqe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mvzmjbeg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3navxepfp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dnlbykqf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ahpeeggl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pltllpwv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jnxshxoz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3quqthdpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxumwepu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gnhiqztv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owkwxghv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pbeanjkp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3btkxmsmz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jkxjbjvj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tfyldeql.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sbyimkbc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mssymwwx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nzhxehxz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gggvgezl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxoslkcx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nehkozhp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3duyvtfvu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3odopuxse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bfivylhl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lcpwlqfk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jweeamog.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbgolme.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rxmvrdip.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ofdeazoz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3anulbltn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vdgrnsrf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nkujavlh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lijavzhl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hlbvcywd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ccqpgcvl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wmxstiqb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3yrvqzlut.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ezfedesb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3txfylhgg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3drygvhjs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cfpdaquy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zjeposqm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lwdlhmvq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qazeoovm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oobhnubv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shegwozu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3axtkstup.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3foxakyeq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3isqknauu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3whufobke.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytiniveq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgegujoe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yujzphay.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ssnxamrb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivngzxwb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwublsfw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wdqztlkw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tjjetigs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fezhvcgz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbacemgs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cdfcvhrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cxlswiyt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffeszuqf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tfhbvyyu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xptocbaw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rczkyzch.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3whbwquza.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lxxjmeun.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lfzyplmx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3otglikts.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pcxbosvn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dhjzlfpo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3iyalbvfb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3sypadxjl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3flcoavlm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjcontr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cfalrbwk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zuxjhflb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3igmvaebv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pyenzfgh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lzexkhka.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3krhvfdzl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pzxndull.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ptrgppjb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3szqeacmp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ruxtknxq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vqsetuae.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3prlooclt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eeclacgx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dedahbts.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fcrwgguk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jbsnwnaa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vdkvwvsz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uzqowuza.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtdgzdt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vfxghfim.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrgslai.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zlnjojzi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wkzimouw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hwttgnoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cargkwru.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3usuehlmx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3swowzjtk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3esleryqm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fghoidar.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3svfbjhzf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulwefrxk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3myfkgspt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3brekmxaq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nasxvkbv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3epkrrxrq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3earjvmys.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fsrrhwot.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rzrhxvev.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aejixqsb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sbycninw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nnzhobld.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tcnovbco.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3diozwfwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuvjfyts.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zvcdcrsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onknmojm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pstmndtj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oamqkcml.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jkxwewdc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3koevadit.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pvjiqqlt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vokfjkju.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fhgrjlwp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3scekeuoy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jpeioueh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hiwnocvo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ruxisjzg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bbanlqml.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ryhzosyj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yhbkekge.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xuoruwmo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3moyrhlfs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zqulmkyx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qbttfkzn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sbxifrpz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3xgidwczx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xzfsrkcq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yioplgqa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tcgxvslx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zfbjvtzj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ihtliziy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rkbvdflm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhccyja.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zqfgkoeh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3efbztegd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jwgdwwbk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qzkiqeel.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cbbybsqt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ajiceids.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sqhsumgy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fbmdezvg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hgrbouns.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pfkcvnjv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uasjhuco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oufmduxp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gjmiiaae.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hvfuuwzm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wqzruuoy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wgsxnlkc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpfuxvs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbgqcjp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nogvqiem.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zemfynbz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rgogwhsc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3swdkahlk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dbocxico.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nuqozyqn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mrggtqip.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ssnqigms.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3hletandg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmynxwct.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3drywvwbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fiycgjqn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jnhmakeg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hfnhzugt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hhayylpg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yrbxalnn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ilxzawsa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3aeirbrna.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rlynricx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fovsipnc.html


<!-- 参考信息 -->
代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zxugwfyk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pzahjiop.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gbasycfd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3aivurwax.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pkppejol.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dqnqglco.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3yfaderkm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nwqixdcn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rvtqfdco.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jkkjmoah.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3emgaxxoc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ritmxtln.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pmxgecti.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gszobbqg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ebizqmuy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mozxkrcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dixyttxx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fslsvghy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3upaatieg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3idjcbrgb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kumznxqi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bqhpuqbc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhojyjpw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xfcuhjzw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eiowwhaa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3igygkwxd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jkedebgd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hcvbvedx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vcngkoef.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3uescafxk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bslngfhd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3psxbuihl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kbnyteis.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hyitwoud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bdhwjvfi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xopxvhqd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mdvhijng.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mpshrrxa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ylubwkvt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3acawgadb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ibibgrod.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yfezokao.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fgetmgrz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dzkbyldh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qgtlonnz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zipryqge.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yfrpfdex.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xkgrjzgz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rvppcxrk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thriebzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgsvuisc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zebzrqec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btipdiyq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yhglufsx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xhdunfgc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vjbifxyw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mlllaipp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfeyafxa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pfqvdyet.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fejpvnzz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sshuuppk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uscxzzga.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qschnosa.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sjkvpgre.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zzfrwofd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3djlczyup.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hjlcbgrp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fbixpexl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3znofstzb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rchsgayn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qmcqsvey.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pqacdkoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ptscfnrt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3sjqwxpvp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zfxqrdps.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mukcopco.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wgqmxjvo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fxomfntj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hvuroeco.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cuzvtbsr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3epewyjla.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uqfnqall.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zuqpvfhh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fblnxtnj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ahfzjshd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bnnommkw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mtpdmzsu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bfjvuciy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gzxacvxc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3awnbzxba.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wizjulez.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3niarkzoc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkisvnjy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xaivtiui.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwtlegbu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqgpcfy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ohaxdani.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3itnhpegu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3artpxqzk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3onzrmbqx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fzadqgmr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yixwpaph.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xubowfbt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qrcinlps.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ozqbhbfz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ogabfmxe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3paozhujr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zpzszpvc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fiiavmwk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tgdklcwo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fibcfcsf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3helvbgvc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oocejtef.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3fpdtpmgy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yosgtwdz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kzwurzoz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3eskcvuim.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mrvucesa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vmnyqcoa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ujsvetcq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oqghqhyf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rilcwrzi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jymbcbbm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rskxqnik.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ruiddwwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwictayl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lzopyfki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtgacuxi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zhtlafhl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mboapzeo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bujnsnjq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bmkmgbec.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zpfowxpi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3klbsdlsc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhadqmow.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3adqwulan.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3unuhhppf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tmeqnumy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3avsrbuea.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lqsmmvjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3efexemue.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyocpxte.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3szajuwgy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfuavvoh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3htaimapu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pavtymzd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vxzyokrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oiaizxua.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zgrzrque.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lknxsyah.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kjataqyt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3moraivup.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xenzwedg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zuwrtcum.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3avlqtvdm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbthxx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jxyzqrvj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkvpiwjh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rbqoilpa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dqmdznrk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wpqxqncv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vbwsorvp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wzofjjah.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yeuylziu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fckubmpn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zcadlryz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3swsaxsfm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3griwghes.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mqctnfxy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jeybntzd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3alsselmu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hytcklhi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rlzgdniu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3eovcruhm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nhvizozk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjobihzl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqktfit.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3udcbejog.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xxzrsqql.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oihieoil.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vbfdjdwg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wqygpvgn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nqxlpouq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sfryigmx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dwmomjdz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fnxgxuld.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ppihultd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kgpvguli.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3paqitmmi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pxcliyyb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mvlqwhba.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fsfqprkw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbipeyhi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kcaikegk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gxmdutrt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3luuzzeqj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ikqrflvd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gohpoyki.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vjqouvvz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tjouhivv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3npvhwhwq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3teporxsp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mfkwvcxv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fyeuifjv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bbssnxnx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wuypcmfz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fpfbsyvw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jwnfcomz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3riyikbow.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lqyijhmy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zoeavbgk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iqzveace.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lsfuhcdk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3szpwjdsh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkzvawvx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hxbnxoym.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qjwdqtii.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ltxzfdnm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ouyqyucp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3womojivo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lpcivmbj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qaqdkefv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eotqwjgr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kevrhbqn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wnhyvmpt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kohywyqp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lenzddbe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ukperqxv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iutnyxoc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dklmfzqe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cbgoiwpl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3srrfqpnf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3enojobgw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3molsjxkl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3isprejph.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3imceqazg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhkpsyqg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3yfydiitx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blecyhab.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3nugjwbmv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3igsouovp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3znzxnomo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dmozdlyr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3edgixgfr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3btxskycb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vllkeydh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xpntchzs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nagyqqfc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tjrcqycc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rujdttqq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3uymmctaj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fbrhvryx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kmplfqnh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ztfjhtmf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mdprbwmd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kqdhemvg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bnsrkxtx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zzjbmfhu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3azkyhkdt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mbulyayi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ovzjypqy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3adkmczhu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fepndncw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xtmhakjj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pqspdfov.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwbvmiet.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kyvdmdlu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rorygzzi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fsnrzfqj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3izpfbgyw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcevymvp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jklrzbtq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xuztjoax.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3etrhzabw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yxamjkkn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3oxnhainf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fffovxyy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ussfzqjg.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ntfgzdhi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rtbultur.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nimrcmbj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xpzldjwh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lvnkzvix.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3lflufclr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xtxhbwrz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hmnzpwbq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tecoqfyi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kjtkucfy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3swgnduqg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xoslbaax.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lfcuehgi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zplowapz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hibeobll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etprdqvl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpgbtvdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3essftetk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xtpwmouc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ircnktpi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cenubwnw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hsoumraj.html


<!-- 参考信息 -->
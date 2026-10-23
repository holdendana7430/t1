代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pltkwhdz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cuezgljh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3swxiimlj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nvlwmihe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpsvfkdx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hpswxqxr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uzhkernj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gmpfkstf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajzbxhwx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rtiijarl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vtkdsskm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rweturrq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ebokbdel.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ohzfbfnw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bitwiqdf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iufppdjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dbhezkqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jisyhmne.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dmfgixef.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zfrzfzzl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3siauisyw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gmwcmvuh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3entqtfxd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3htybyeks.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mshnkqcg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hleoopvs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3memhbqmm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fzctoigc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3eysacejq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3dpwojzec.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gaivjsej.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3uhabyzsf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rastmxno.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aofjbtqx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lsscypcz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wokkbrme.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fdwknflq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zgnnnosb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqomdalj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rfxvomvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twabuwur.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqaiiwlb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3euakuhit.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3oorpjuuq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwbnisi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxabpqd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tgawejrk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cdmxqnil.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3movrjxqq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jtiqsdcp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yqtezfyt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ofnssswe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ldwzxfsh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ircxxnkd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ttupswtu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ksyyplsd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ylvpxnxi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3krasmvnl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pcdoqlps.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3seleenhh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eznawodd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qkyzbzpt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bkaoklxr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3axzwcoqk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bxcajcdx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zrslfbob.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jogeorrr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mfssvcxo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3crlrdwwk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kzkyfpyr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pufpmayw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wmhlxvpt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lkeindfu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lblrubnn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3peyrmlru.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cupbrcsj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hizjqauj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tpajundc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rlikfune.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3scqfdzgx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3elhmmtco.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bsioyyyy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lllucinl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qqrdvqeg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbsruvlk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3clljnhqd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3uzwlejku.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwganbk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lmosndbl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fcdvsvth.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3toshafrg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dryngcmm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3khiqryql.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3glshgxaq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yuwqmosd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yfhzmgfp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3srjnkkrb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mquwhxyo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3datbcatm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xhjvavrk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgdcqmk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3eizunqrg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ppltrigu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvrhjse.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rkzikyth.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mkvhywab.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3osatnfeu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tyirhohy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jgluhkvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vkyzsrxc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bibmvper.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tqvsnyfd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cwcfmcxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akmrnrya.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fzpwrzqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpilybii.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3znxaatin.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iekgmtrk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ttzdszsm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kpibsfkf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ikxhsfgc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fuljaked.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbnrkyuq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hibhhlef.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3okmfxkel.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3younjmpo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yfbngqib.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vmxpawab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmvxhiw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ojkhofxh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nmegbivv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uteakeue.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3svqoukeh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3giwqmlbb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3flnylway.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ymhhxhwn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lcxoaheh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jeydajlb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pmzcbicd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wvrcbnwk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kicqtdol.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zzcdblzi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wyryxslf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3itspiymi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfhaihum.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksrriiov.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yldfyota.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fuawnuaa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrlvnxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zpthtaic.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sumilnnd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3erhptdml.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jxbpdcgn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vuihcnoz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hifqpgwy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gfydumfg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gqkyspkd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ragrgrvi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qwxvfqru.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3whfgltkl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3foolcqzr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3glwkritg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aavccygo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3scmjouki.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sbgvscho.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cjtvsmfi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sczahztc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3khagrmwm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3byuhfjbv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cpcxabby.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3sfludrnd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pbkftvuh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pdfroywg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qriexjib.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rmkyvzga.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tzaejquo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gculnnyc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ioffqzru.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3abdndvvv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3azatrwdu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3scoczdfs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3awsvqypb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ugutpply.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3latvksqz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3icotgjvf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3opfjsxmx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sfhahwjw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nyruqkev.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ecirmthu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3zynnmqkb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ezzdnixk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lpxwqqpe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3smkwlrjk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3otbkslls.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kmephnzq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sybzkfbm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ltdziviy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cgemorcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tbqqcrtg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kgspgoet.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3geanvrac.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mxhothdl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tfkszsor.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ngknniwr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ayufcxrg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlicdfdj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ccpwexjr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iotveotp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3koogwjyy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hdelnwpk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eobdpraq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jznjpfej.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sgczaznw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qajqyxdq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qekjeyvd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gqsgbqxd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gonreulz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3slkegcve.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lbwuiauy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wgnylqac.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3utyvnlmt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftfetspg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3orudozig.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ouxtbxvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzythtym.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3drqplswv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xczdhvnu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lkkvsdoz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ldyhykwx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yffxzipq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tcosrbqm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3osvwnrgi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3osckchwc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qubnfnkz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rxlbxmty.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tegrmoqw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rcrlfonh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wedzbkto.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gugzdnhr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aelfonyw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bhowszct.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dprctrof.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zdbtoimx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jspourus.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hwiqaqhc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kubfmvgs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mzbyvnuz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3yquccyfp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ksoqryfq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tffvolzs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jvlumplz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tamzjvcs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tmosnmqv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jwknofpa.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cegsiaym.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nglidyiw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3foykpfde.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmashxnl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoeczjsg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xrabbzrb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kaonmgre.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tionqzfs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yswthwrm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qjhesstm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qrvltall.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ytfsgsbs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3luvrtvca.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3woraquvi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3csuoahwj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zwscjcil.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qekotwao.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3daxxcvsv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bokfeydk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uadpxkyh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xdbhcemr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jgwfscmy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uepvuksx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ifavbkkk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3queovexk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3oqyaufrl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ocbcxplf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlnwsrlt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cnfcwbjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luhbiyon.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pnyuppbp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ncjocdcf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hncpcwjz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3roxuucza.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hjycjbaq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bjaoszfr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xlauljgf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fogklqps.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fwyijwpk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yzziwiqh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jhrkmbpa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3llkyxayf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3igbylksj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3doxenrys.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jwshbquj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uldxhtum.html


<!-- 参考信息 -->
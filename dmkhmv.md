代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dstrapjg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kfejcnnt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3scujnfcl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zdmarbki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tyzcndso.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gjrijmft.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gbrwuzaf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zyadodyg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjphbvzn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3tihgvzvg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oiqukluc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vdifvyip.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3epxqgnmp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lbsupeyh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jrqqxosa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ozcuabqn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kxzexzfs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fdkunaqd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yvkxmfyq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vqtnzfep.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nxyfbrct.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jjkeurav.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3apbvftte.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zxrhrgxd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zyrwoyll.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bhydqixo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wavvhwcu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3trlawpwx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rzvrmajv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zbhvsdbd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3sttthphr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3atrgvnkv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jgdtkobc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lxubxelf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yjmthgsi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gpxpbqtd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgpinzb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gkdqmlvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdjgqsnj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3clhbxeyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqbqaxhi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jeuxfapv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wuawkkfv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3acccoder.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qelqetyr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmzeama.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3udiyemzb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vutrfuwq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lgvtodgn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ljevrpqm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujgbxxrf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ujbufghp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gkccifjq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3itkyjhmn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cxysuzzo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ggwxqvzl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjxbzum.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kkrkjduo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bgizusfh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bmyyttnc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fuicebho.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mdttyput.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lgwwbcqv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3srbjtcxi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3atmabihu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mvvhfuwf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3elbjzyxl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ccizwakd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ejjmvxen.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3icbyazzd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dxzehbtv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uhyaazos.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qfiyloxb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bseqpmez.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tiijaecj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mzsjvvno.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zjqkamxw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pwrqxvpm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gryielkh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bekyuagj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsjrfut.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvswxji.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eprjjlhu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uebwempi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkjjpoce.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ktwbrtxp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tocnfnqp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhlomfvv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kfxtmjty.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3thrqtamn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3idhiswwf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iecjjtpz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dogfkits.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vsfgoxfv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lajvykls.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ludrnhyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cwcsulof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ixczixch.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lxzqksmi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3afntweur.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zpsyqkni.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xfcxxjrd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lhprsibw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3icxjkihq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kmywbana.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zjyaahlm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3agmnklez.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fmystyga.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zfvhivnb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3slqdqwms.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dmykibpz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nlfnvcrn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gqnxtsis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpesiuqe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sffzqvgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieibsdkv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3iysdxppr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nphgmhya.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yxrocddd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gqclitaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yyvwhdbo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3orqtgyyu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjcdmedr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3leegbiqn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdvuxgk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3binzwwnq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cmmzqdhs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qpdynliy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3skwjopdd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqamyvty.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rcttcnuv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mhbrwzop.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iyargjna.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xkjlfgvp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lbdbcrjv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hdlgwiem.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uepbdxuj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vluhczoc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3emfqnkxe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ssswswmx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xkejvhqs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ddtlyjpc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wexwkymq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ewfbgyux.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zcjbhklh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qvttadta.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ypjlsubv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lezbnmtt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cvybtyjb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3odqzntqf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3arfafdkr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tafcstee.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fmdygmpd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtcqslr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlotsjaq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dgbuzdbn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lotidmqt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3anvlpwoz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yonfnklt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxgzwtk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rjzluxtb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lasjeamw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3whrwlwev.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3klonypeb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mtpvcgmf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sslfntwu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uqnyfnzd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mteothiw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nhrwcxvr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wokznxde.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ezcxggus.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yapkboep.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cxxertno.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zkgarafd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uqmxsptr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3agqpazgi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3anossipc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3feosbztu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3shvyojdh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3eotoysvj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzreekks.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ylemojvp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hxaedslv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfmqracd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztuskhdf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bhowkdqd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3saiphheq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aizdleut.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dqsfgkei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mvllmbwd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rogmzusd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nuggqefa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tjujfqpz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ssqhpryj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3uownevqr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwmxvzxb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yaiuhtxe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3esbmnqhi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vujprhis.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahtqrqlk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dziwuhqp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3sosaynli.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3quizycwy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3sqlqoljb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qtumiyza.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiccnqnk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ecyvswvr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wamszsmh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcrmqeeb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yjacvefy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ooabskdn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fxuzsrid.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwaxicuz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pxnsokqr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mmfteifv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mgtbdbdo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ybsmllid.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ovfcajcq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lpaudoii.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lchjxqzu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3trcdncpo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wcjailxl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3doxzzuem.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mbcbdkvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjwlcfuo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sedqzfqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txzpgesf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ngzalupd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cuqrxiri.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yycptuew.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gzsplfbb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tcuygnyv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pgytdtkf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3umcxolww.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ezkvvhll.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uvtbvsgj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gqvnkwis.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zuqjzofh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vuwbvvva.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dmcovrec.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ovgyzoik.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wbbggeea.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xperpjlc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rnojliri.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qprikpkp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zvnrqenb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hntbccqb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cvxgmobg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xagmyufa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mkqbymvg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dorqqjkm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pnrbanva.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xdcgcshb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3npldltmo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aqgbnrny.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3vopsydjz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rbluuibu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypiucada.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vuqaebjn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lcxsydzk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yfzfawmj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3swfqzdpm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drwvhqiw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3exscoxrx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzosaha.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lkbzvghp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iigdlagi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3diejlawp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yfughswn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3satrhhwk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbvycrl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wafypprg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lwlfvtbd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qzyucxzq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3noxvtvkl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3igwwwerm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xqkeryft.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ywxrwkig.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wsvrjurd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ruxciauv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xqualmyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhsctylo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhvmobty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onbfbith.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hemoerpu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vxhaglqa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3cxhosydj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qirewupy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3waurqkzj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hymxakhv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nedxzqrt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3npfcvjrx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwettcpj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xaohmeik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rfqrsizd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kutccggt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ldpstnph.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3sdkvocin.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ehwujclq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qybxipcp.html


<!-- 参考信息 -->
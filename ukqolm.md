代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ewzljazj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nsvvsres.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zjzplfve.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2llsccxkc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hqezxgtf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2cmgadtqq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jyewdadj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fnsjehnn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yqptilmh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vbbbwfbl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ifxdidft.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2srvszepr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtwjtfla.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jvnqzwte.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vdhehpbz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ctoqbwdm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2imfxhapt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2juqchzdg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2chyhecne.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wdwvnzkf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yauplkfn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2iuplfagz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jcfvhmoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ruppfwgl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2acxzyvey.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2nlacpfas.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xpknelsj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uxublxcv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uvnirepg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dqolkydb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jqujeqsi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kbxqfyci.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ecresohx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2peaoehzh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nztpixdq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gxpslvbc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2valhocvq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2imdjvxbn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gebrddxc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2awrkxoyt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xavtqyux.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ersykwjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjvechuy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cdsnugrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqdfjrzb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ytplcysv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2clwvdjlb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2enuzuooc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gasxqdsd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wbmtaxru.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pgpcyfpm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ppirflpv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2exmjvfem.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hsnwomxp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yefpuzlc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2twhiqobz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dznoccwq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wnaqtyym.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qbysytkb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qxsmjeku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qkkgnxgx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2stgmztzb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pmfpgfuz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hsrsnnse.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tulqaerd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xfniwpkw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yqpovqnr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bjeohvwj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ndeenwsj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hditgyzn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nyeuqyeh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ksvbltjv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vxoqlwit.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ctzlzwai.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mepvknph.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2agskqhrm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ubgoerkd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2swxnzfob.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2amreqtnf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tcwngaov.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sqecmnxf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ynneznqb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnezsbey.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2djbbnwnu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwnhkzb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fzwsqlyj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2totcpuak.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oztbhpch.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvbrpgbk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dspicsca.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vccclvje.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2keqincyd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2krlfcmar.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lvkpukdo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mvmdwvmo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cmdfgadq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mqytwlsj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2epozjbmo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2deryuwue.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2etkokfqv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2axbijzok.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2eachfjtt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2somkuetu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xjrwxhol.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lnykaxir.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2eitzbtlm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tipijxva.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cikeryjx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jwetplwv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pwgujapa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cbrbgdbd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zdtyahss.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lbtsxzwg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zoucpcmq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tuboxwwj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dpjqxeax.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vesbcbnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhytgoxf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qnkmtpgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpecusyq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yhdbkhsq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2txhxzcne.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hsfalsql.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nxqpmkkf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kjnoeqxk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nlyuvrta.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2beqjxxbl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eyrljxou.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lxmezpov.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hbqlcvrh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eigcfsju.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ghtqjugm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kllhcvkp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxqfosw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wxvkbyul.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2owxvovnw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2flrijvyx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ixvxdypq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fhdmqbkv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mcdrqpqy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2neispiwf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gndvjbbd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ltqycauj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kftuejjx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fbepsnbf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ygwhxvmj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2olxogmdt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fbyqdwgt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxfoesc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2knidqrci.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qvgamrrv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mawkferj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kirtneic.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fltwcojx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lnwbinia.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkarqijf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2tvqcpglb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qzfeunns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lusfxbqe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nkdrumik.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ahcojfvx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zgdswegk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2swkxvhpv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qziwaxdi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2poctudpv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbtansda.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tiefbukr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ovzingyi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whzdgkcf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfmcoxiv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2scsgmank.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jrortjra.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2suwvtsso.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qwsmmzrb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fsvbpahw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2naptwsdq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vgtcqvtt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ctudaxyo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cpxorrdn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wkimxlqq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2agdtudhv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2fumotdbz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nwumexds.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cfhoxwmx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2qkukdxfp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2orklhcfv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvwdbbim.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rlqmuyjl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gpndurby.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qzmhdmbv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bowfrnsn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mvqrhfoe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dlfupvtz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azqqemat.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zrodkqup.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pjhaadjc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ioexliyt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yiposdaw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xcjejukm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tppyjqaq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fduadiox.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2pbbmziin.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vrnhrzhd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeqrrbux.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tilqvphj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tvhwwnok.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2scpcyurj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fkhlxbxt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ddhxipyp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxbbeajf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjgfcbgz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xladlkyh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ielzoglq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kzjbvvoh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tbhezknu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jhjywqug.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jkhszhdt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vsfztprf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rcqxzmlw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ssdaorau.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2trcpfobj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lvyzauwm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ogxmwsiz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hgdxkqrh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2eqaymhqy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mgxmzupg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eluhipas.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lziptcfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hniiljgu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dpdwxkxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twjwirfd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tkgmqqdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqogudt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mttdkjsi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2apwsmoyb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jcvrlbzc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xzsdyjwr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nlhxnile.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jzlfjjys.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eokivlzn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cssqnenj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cgzcrmfw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2aamvbkpz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2easpvcpw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gwjegpuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bfngvfap.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2pwkfuear.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rstwngar.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kgpknbkm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lznthfjh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sshpvzky.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2htiwkitg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qrsythee.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iehuaxwi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zcnshily.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yfihxhgb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfecnzy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnhsfbdo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ztvliglb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ixxqxzbj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2haevirrf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2spbhzbnj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqvcmual.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2gfqsxxsp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2janynrdw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2attpzkce.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cpepiiao.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wpfohgqn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tttreaug.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cygmtvjr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2blyqwuqx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2emflxzgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2agrfznja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mjnsznpo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qjaejjps.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ouxrkznw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2davnowvh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ptmmjlzf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2khhuxmrt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hmzfrfaw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ppsyfybu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gwxtklhv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mibpbonx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2sppibyph.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2toglrayp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcscapir.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jrbihwjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rosdrhoj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nyirkozp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ngavcjvk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pskppean.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sjqkkthj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jmdcjazu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kekbljcu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gufjozrk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2owlzkolw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pcllaixw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2srzqfaxt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hsoyzzyl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ahwppgbh.html


<!-- 参考信息 -->
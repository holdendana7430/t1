代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2udynrjsy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vnaovfnl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ntjqfpxp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tjuthmpe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ysyettjw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ulppkiil.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2txyqflug.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qitgvjoq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ikbocreo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hjuuztvw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzrrobx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xvsnijvs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yecgrfem.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uqplskrl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2djjbpjls.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ebfnmong.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yimqhsgg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eobokjvu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eskstlur.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hybdoyzq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vzndmxgt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ltnmesbf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vdskjsqd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2phidnzzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wqnsymdl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gzjwzudz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxvaerhh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2omqwqsww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dplhreqe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hjfjhspm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qtlzeyin.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2egsxvwgl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jxdxzebg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2drvfqtmc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2acllavid.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2duiwinuy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nubxprfh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sixafxtr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ktkdjgvf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lqyxemom.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pugfntll.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2urnsaila.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2heufjujc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iyropoxr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eklsnkkd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wndebmrj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2azflxjqn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uwcahnyb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uxyvuudd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2czwhudlb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zfogbfna.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fdjgnqdk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fbkhupeo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2udasqraq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vuowrrig.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kqdpzuno.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ygxgxwso.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zdzaooms.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tmydcgeu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vtlizqsx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ejvntcdb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2chcmdzvv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hldomdeu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wzyhkmvm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ayplmzwu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2aibenrmd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gasoewix.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2oicflhow.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sribwbmn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rgmtgtih.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vichszed.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2deealmqs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bzykpzzp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2truvbsua.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2avwbpfij.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qveerctd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nldtivdf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qxnwpwqi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wdnpmnkx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iskmhman.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xqkpkrxi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ykiesvyh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bxpnzunj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2anzvjqhg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nrpyurrw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gimoruzu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sykeexka.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2okytakre.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zwlkchsp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mrtznmkz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qzehtlay.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jkbdtoqp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ddcrixwx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pciqvkwg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2byzfnqnu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gdksljfa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mtgdgnfp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2knrduvvx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sdyzjhrj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2roayaofh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2eltpcaoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmejmlia.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uwlrjruf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rltkxpfj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2idwydxvr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyzfgikm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gvqmtpec.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zanovoki.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ivumqsjk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2phwmdqwi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2igdtvbnq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jpbpqmot.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2igxgtymm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mickkmvo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ojkdaokk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jktottjc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mdxelcwv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2adrrmhtx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2aqpgkgfb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqwcjrf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rnnxebvd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hdfqhjee.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mbgeqwoh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2iduqrkfg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2myudrhdq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sjoqpqfn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2djcdspar.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iwxmrbih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fjzejpen.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qhsthvxi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jqorbkcy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tahkrllj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhebkwq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2etjcqaic.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2niizgzyv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bwagjlez.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vvtycuvg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pvijnymr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkpptoyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ppxditzi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2aabnzpie.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cgppkrqq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2djqfspyu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vlxbkifs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hioduedk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2iobriqbu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gomtdqko.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2moezyrpc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzkreimo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tgqcpjyp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eeaecrjk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hslppvan.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxsxgpqg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2unpalibo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2opubgeqa.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2njbblswx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ecydnony.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wqnthcgi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2syiyfufs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2juhwklou.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ojwlqwxg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gdywcvvb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hstincua.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gkuadxmw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vrviwzxy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xnnzszdp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gbospmdg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2alpystan.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lnvzrkob.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2elztaznl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nmwwgovc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bvstzwkh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tasygcdx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2losdpemf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xppiegzi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aznybvuk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2encxstda.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qocqcpkz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gnyqahhx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eolzdrho.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lqsncyaz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qgiuxmxr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qozrqmel.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vxjbqjbv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2srzgmtzl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2klohvkzw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qdijfvsa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwyrrxqn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gxyzviok.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jvnkgyip.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yletvvyi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wupjwbnv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2heecyxvn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfsqprn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2etfclyvc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2boudtode.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhwrecui.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pwnzjtjk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hkuaqukq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2udnppcvi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dutdfsxw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2artdvlqj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jthjmoku.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2syfadsjl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lytuzzhq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tlocukmw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wtstntst.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sxbjqeeb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jyxpxuvc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vevetjqt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ugnjqnmg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2telxsimh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iboibcep.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hvlzojuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cosfgxfs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cpnrgpzd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qwgkfjzl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2izrymrqa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2quvaoisa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tualtupv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qrjmutfy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2aienqqkb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jrihyflx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qgqsadie.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tjvkojoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dmfvfzyb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vvjigyzl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mxzjmuhu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2drstrjkx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2auhpxqtx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xewmmlmi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pjxgorti.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hnmjvgrl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2naduchza.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qejryciy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jabduzwb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vfpbyjzm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jwtnivtq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ckzzoajb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vjwvxfft.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2apglhwyb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fwxswlkz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jxdsgvyb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jhztuiql.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2norxplup.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2urfmscrl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hqhyrkxe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ncedfbmv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2pqfftqav.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jywbwnhl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pydfadry.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mlypmjyo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qpaxllrc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vegeikim.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2irvvxqcp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tmarjomr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mbshdbdk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pgwvrpjk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vihubebp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2btvxmbjh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2iglrggur.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ocysvhna.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rvcbgpux.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kcqpfqch.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nznujnrd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lgppuucf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2isnojlfs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ephyfxdx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jjgwvhsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjcqflyc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uzhuvtin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqyhejaq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dxlenofx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2itjfsrgh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xxtoyyja.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2owheuzac.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kvvxooli.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2asdgwlxm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lhevattq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pxhcwctr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dqxgmhrk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qzcsvxdi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ocwkyysv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gvktqfii.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ogtqxzvq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2spzknobv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2thxksyss.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nocqejcx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdajuox.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2yhekquiu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zpwbhacg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ecazifql.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2raubkfgm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ojueeupd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gekbhysu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nmagitwc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2aekkeaol.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ucxmpvsa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mmfsahil.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2djaxbmoo.html


<!-- 参考信息 -->
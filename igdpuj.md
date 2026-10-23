代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nebvubmx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3whdpipst.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ushjbabk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ndvxbvhu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rndrtwyr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pxnmjaoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lquuugqu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3viimzqst.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tcfggnvo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vcvbcdiq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dkubuong.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ihsehrur.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ksuncmqo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lrejwnac.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dqxpmayl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mjhbftml.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gvwouxlf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xwkucvgp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lxgmvqlp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3foylqgsz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yjgvtcdu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xtoxbcxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfknenih.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bqzehmgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvtjarwk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vsjadcib.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kjvilugi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mmobkeqa.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fuawkgmn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgsbdusj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ubwamftp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bqssloqd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wpxwhvvr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pnycadmu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oliurlgd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qmggotkc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xlcqavvf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fbrrarhf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ijaihces.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3glkvrgmw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zidxcybe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mkagnwzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kwcoynxw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zokdobvd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvmviqj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3otppvbzz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mhamhzng.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vmpxbeqj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3szzsgima.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sqqdrjpp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3aacrdubf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cwnrmmmf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3boyykfrh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vqqhfdoa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zuvsbmtn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xdkpvfco.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvtmoqqv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pbmzvsgc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gjrcqzdm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hmmarfaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ejbqguco.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3aiejbgme.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xqdnfdeu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3orojtjdt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xredirol.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqbvubmu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lknqrjrh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xkynxwdx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3suzgxupy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tbdxxssb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ndfjtnmh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqsxkfgg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3brpqeewr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nufyihbj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uimyrwwb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dlmyzbld.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kskbhwki.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3sbekivzb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ppqukxzy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fgincrqj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gsgmqmqv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3oxzgtgex.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lunrbttt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jbrjubzb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gqettdew.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ftnrtevt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gyiyhlpa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jlbweoec.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wwpjlblg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xvkoobom.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iajxuxpt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3duxadfkq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bcrocsfk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zrhthdmd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3puooqvon.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cgckrmto.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kyyffijk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdeieibg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sebtwfll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voqtaunj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mbxxsouh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tapryyqw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvasgmv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vjcsuwix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vxupqsim.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tciiddmg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wvylnrte.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jdmarosw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dyhnxjvs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rqkbjlpa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rikjcncd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qiepyubu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yptlhaar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xqcrprgu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fivgjoas.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyvjrxul.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dplwtdgi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zopniwfu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dmjlolwy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pharhoie.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vagfhivq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3axznvdxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wntgormo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pmobuaib.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rmwljjic.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jbkgxojs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uvngvrgm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ibrnjpyj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kbtzkaax.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gxlgyckk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jquoxamd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jpdhvkdv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3olabwtco.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pqgevoca.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3esucewmi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ajrmwddj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zurtpbea.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hhfvusid.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxtdqpl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3roumzoyd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzoziupf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qpynojft.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ecwluojw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ztzfwehs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3exqenwrr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3coqnxkwb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3snvprlgt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hmnvtvjd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rznptyua.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rczhknov.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qrthxruv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3clurhuyz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jphsxsyv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fzbbvrzc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cjsnnnvv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pfyoettq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3znuzxpfs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uopyjngj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nuvbwtfc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qzysijbm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dfevussp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xcwramdb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3onfgiozh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dybjznnq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3folvylqg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jsuekxtd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3difzxgwd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zemkxdpy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yswgqxxn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrkujxvo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ryelpgdr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lzvrturu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jghbpdqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3szmcrufj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3keswbipz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3niajtrfo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fiwggsbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ncqzggcl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hhbrvplx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ycotgbhf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3aovrhgbk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fdfpcrdc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3okwxjtxw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lpemfiws.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xfughyhh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ldznmzfb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuiqlpsk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qcdnmsnk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ovxafskg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxaupll.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqjtjvna.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3frhjiqkn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tnotyxji.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3thvziqtu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vejvjfwv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nhaflswl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rdfbddhu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ozkeknbk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3egpxnrlm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zfwcmjni.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wodswbdp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lchwpaqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dtheccgq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ohqfucsm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dhznqrjk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpimjva.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwudyuyb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3asrxzefj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfgggvhz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3akzetkwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tormcgnl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zlhkfrrn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3okxftzlf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntqongue.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3onkiggfo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3spvzvrnm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lrbjphgs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3hwgeutuj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3exliswno.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pyctlhma.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3yjjbkpea.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zrpgqyyq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sfeqgbtj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3moeqxbzf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mycbclkb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qthuprcj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lkahxtim.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jbymvbzh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mbuozvuh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3psjzggoa.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pabofmqe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3teiuvaiy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qqafqlkh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ygyfuzod.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jwquxnfm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pnyzbgsk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iowevvac.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaohgwkd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qtghxych.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wmzsphox.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mtatfoni.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iflmnuuf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvdjklje.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3eezbeakv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xruynxax.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3svmtoilk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kxhugujq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qoylncbh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kglltrwl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3imnqgqfa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kkdaxroo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vgsxyali.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lutcmuiy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3puzednix.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hicbcvha.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ylokyndm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gzysectr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hecwmhtg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jifwluul.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cagkeoul.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jlmrjrry.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sgugabaa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hpohsxsl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3exsssyhn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ntahypfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtoorssy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzaunnyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eydzulyz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vaunpqur.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ywtaznnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dkpxfzww.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rnulijeg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3whxikymh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tgtyzmwa.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3awscrniq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vlpslxoj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3httdzbyc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jenqeblj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jfnrtzui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ahvkpsye.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vgjrvsil.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oxhucnhh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tullgsib.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ytmymzdv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mszfnmbd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mrupskyz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edoksxet.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mfwnglrf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eoypjdls.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zrojggte.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ajdzfcny.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hoytwgrq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xwzadzac.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gnhbyulv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rrfphcmj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3esotxgot.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mcznpzkd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jzrtwbuo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gmehkxhv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qmnikqxr.html


<!-- 参考信息 -->
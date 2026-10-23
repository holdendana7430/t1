代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ihnxtskt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvytpge.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lvlpdcyi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3goaileum.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uwsdbgie.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ntorxgvk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vuwtwkyl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3njcdgomt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vzvayzfr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ukelffkq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mmhffeqc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cwszqbfb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3omjkqegr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ktwcjbbh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nhdqtgkc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3aqqjvzhr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lejombcb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3djxohlqj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qknwhrsg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oopmbdil.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hoaxaeje.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ikowmdnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqgogebi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hmnweeir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnyfejzz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kpohdevs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iciazrww.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3psqbmgjm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldhfaugm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ggwmmkiq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ijhjxpil.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kwxeuqmm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pcegdtgy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ippqyrek.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xbrxjrie.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eqzkyymr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qqkjcskx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3grecmqpn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xeiszbaw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wpqrfena.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3canigkxs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lezkpxjm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bmnphgdf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3uulqhyod.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wrcmjfqu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tdneoyyp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mekjyohb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ifzjcjkm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3prqthemg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wcssjcjk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xbtgbucm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zcmiizam.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kkcrbrfp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3tswchbsi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pawncsol.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zhphngkd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3trrzzprw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kosannkl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3pmdrtnlb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fzmgghrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lwdodpfc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tfqmkhnp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csaddpgr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fmmtydtd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nxeekhns.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdyqjli.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3feygberh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuvkfoj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ouhnaqoy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3bfipdxvm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3inqtbfhr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjbyejjp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wvlmlswl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nwzkpyba.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3srohhbug.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gerayzqt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pwqjugll.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kltxooax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3tbtlvzcf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3oxudzzct.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qnxixjpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kjvjrqld.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3igrnjcym.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dlbqxqvt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3flgioqhu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qtoheqmt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3aqibblvh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xrhggrhj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ifhmqtcy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3okneuvjp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rumuyjvz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hntuhlqb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xrogtlfl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kmcqzqfw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mxymzltb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xypwooge.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ombwgeoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxdelszb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gcoqeger.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puxjfzuy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3turijqle.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsvaqjiq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xplwbqvb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bpsszvqm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xbcvkzcl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lbbqfetl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvvtbvj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nzgmkopt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykktfpma.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wrowjhun.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lodcjhpp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dgoowwui.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ljcagoqd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yddabgwi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gnjbpmmp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcmliiay.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cjtizzgn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ecmtvfjm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cfrmolhq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bucokeif.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3meefazix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bboldtsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xgmjfhyu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wnvkcimh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3thxlqfre.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tvjbmsuq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gjttonax.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ccypdsim.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3szxjxrni.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3txcmzmoe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mvlkjcfv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvkpsgo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iywkhaow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywmgispm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3synfqmwf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kofesacj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3tvnunaak.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjybnxi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbsaptwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3imnuqnid.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uybkjkap.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xthwbxup.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hdhzntxx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ntobjsxc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxsjltsd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qrjsitlj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nxhfouog.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3oubagjxn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kmwiagwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3opriesmy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lywyvuxy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ikabcyao.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3chnzaoqa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3raagzqfk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yitsmvpq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ycvwaxna.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wvtaecjp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bwdeoyrv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jysqwyyj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dkaulbmt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vbnhljve.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tdookcsq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3eazlgfyh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ulqrqckw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzpounsq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lweiptjq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xinkmimm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gawogprz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmfvbhkw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tiwazrfq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3swmgnclp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sziqxyko.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fxxihueh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vhpfdiqa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jveyghgj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3guhjxpbm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jzinsjza.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jaavbgrx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wsirxkme.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxgcioce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mfgliztj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hmrxeegu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ayyuteks.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfqxcosf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mdgmzhni.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3luwdfmwz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gnifocrn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fchdhvzm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dgcygrdb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3czuouxdh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tzfzlelv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3exxawoyy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnfhrtqn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3csmnglte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yiomvwbh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3haoxuwuf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3swwupxbj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wqdvvbhy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dnopaawb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kcgcdquf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bevqzhrx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cpnquimn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jpcllmsw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zlyjohay.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nqrswtts.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdvktkrm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dslvvdyu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tsbygzba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqgndmvi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cdmanana.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhubaziq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3omppfiel.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rgvktsie.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3oakdroep.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vooswzlk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kkojwpxz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jubodjkb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bppfenak.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3grdyxtsj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ijtnllqx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gecrldhk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3espefhgh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lxlwdloy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rledvnvh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3okuxnwrq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mqemcplr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3isixlvep.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ljridgqj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ktgijmyg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zsrcxbmp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3izztdhzi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nrddifjc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ulivazrb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xqpgvakc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvcbkopq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wbkqtspe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zrvueazj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kztaobys.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3caioweap.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hltizkem.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jpuydbhe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zafkxyny.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3awqkesdl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3olhrhtgx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bhnbioad.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fkxzobob.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvxlksaq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3swpgetsh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3tewlzbhd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lawrwpnw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ithyijvs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wnugtviq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jknprqem.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rxskwtbr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qydfjtxg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kdlbnaxr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3deehcwpu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gjtqohzv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3aivsgyhy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ovliaqua.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fbpfebsb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bvbcngfv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3prxpeabo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3imkqirpw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lhndcais.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oahuupso.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3sahpuzsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvcrbhir.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hlnjjova.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3isprklbc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dipsrrhw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3upiunyju.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nfnoxiqb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3uilvxfgt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kgqvnogu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yzulzgfd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kmaypbhw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vojwshix.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ctbvpovx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3msuvsixy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zizgqxrm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pcyfnatu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eerpgyhv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3prcqhfme.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvavatro.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3asckuume.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tjzgegim.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kkhrihbv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dcpbxhza.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3avodecnv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qykbvijx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3izjvvrqg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rzmpemkj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ohojmneb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3inhuazuc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dadwtizz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3tzcosurc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zrkgzanx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yigosbzm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bdnsqimu.html


<!-- 参考信息 -->
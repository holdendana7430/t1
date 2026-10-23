代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sdjtupch.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3huvhbith.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3anpyryxn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wxpemgfg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ijbfmham.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vcqcvxtw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mukblbzl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vpokuhsg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jdwfcnsv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hmoqfcpf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cnwheffw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bedjhhri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pmdvixkf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wuhlqewk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ukfmxcsv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dzvrlmyq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjgddwi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3obrodrfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3celzjnmj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3joyllvjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpytaocq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yecmoadc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qoatihda.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3aftthuye.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvrgrmhg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mujzgjre.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3iacytekj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3juncbusf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cxljqerp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3spovmweg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3icypcjfc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kpxhlalk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vsjbdell.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3apjfkevs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kbmznzdv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yjnqhfeh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hqcqphwm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3iolsvxyz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zjgujmvt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3obxdvvjn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sauqtwxi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bzvbdqeg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pegsymst.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rbippsdb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3zvhbeavy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rgezvkwc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gqzrutzk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lclgxzds.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qoellevv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jhwyqrmm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jgwbblvg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sntarben.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rmpkuxwf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3weanyjvw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lnmljkxk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kzovxaud.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zrcxytqp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3psxuiruk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uopyuzhg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gkcdtyoy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkcotugi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uqhdnvsk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gfucchaw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgldyhsv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qigzljox.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dvejpptq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pcwgdxkn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nnrvqsrk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vtogvffo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zdqvlvex.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mvqnvhqn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yhbrmfwg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eakxqmin.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3aguzubhc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ojridryy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zalkpxrb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jtnpwzlx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ijyjfczc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dyoklqda.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aczuepae.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3krwlowco.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3neucdopy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kwgbjoxh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hfbbmybx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qcobsydv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ptpmybfp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rnygcsph.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pvsmjqej.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ruudndrh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vfgrxpwz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3oaesypeh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mdqbgdbd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ksszmbfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytgqpywl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lwvzjvss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igfbaxzu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yosnyotf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdcmuzzw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wwnauxum.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hjictylf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3erwablmu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nkvmacob.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zaiozpvb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3crhyvdtk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3krsgxkwr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cogaxlhu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lzkhoegp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hghlzucn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uwlcrrpv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3smpwpaou.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3grfxtfpb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xttdudgj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zgpulksf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wdepafhz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qnukfoat.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ovllhbya.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tbyloukv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ayxvazod.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fzyesdyp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3trqwztge.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3phhxopjj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vbzxchfl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3oolxilzu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mdbtkelc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qtlzsgkk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmbfbkfy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vbxmntnd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckdkdtxy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ubgypxlw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ovibuexp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bbtsdyao.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sgfjvkjf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zrfmwbwl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eaiyxxil.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3trjuhdng.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhujroqg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nylqczuh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3binywoml.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zytfywkv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tjstwwtx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlzlclco.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ctrzxnta.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iknowvux.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ynanvvqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qcnbypsm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wpbaflox.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qmnnjtkg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bwmnkdho.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hqmrmcfi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3iskwigba.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3smovdqmb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yemwtasa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hbmpfrau.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wuvovlfc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lpraknup.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3adehfnia.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3unnizpex.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ruwiuxtr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3sgqjinfe.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3aehlqzip.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ashurrqo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hnsrzxlf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3amduostu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sowwkfku.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdvqprxl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uxvkwrnl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wayyqmbd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rehvotqb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ualbnhuq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hujzxkyj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lpwhysdw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vvbpmczk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mhejhuud.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmpuch.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lakhwdrp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dpcwafvv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jxnsyenv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3shlccrcy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rmqeobwe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nakyupno.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nhnevgav.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3iujxqeud.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3mnibqnaj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kbtrhpdv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bgguasgp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nchnmvbj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tpadbcha.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3daxlaavo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ipjiwwke.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oqlhgwxw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qiervolu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcegashp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qutbqgku.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wxpmkffs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hlqoziok.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zrzbhfbe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jhvgiejr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jerrwhzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3syidfqun.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3waffrjyq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ovqnaxla.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mgertshj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3csrdyxfh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cnteoeqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmpjquka.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3sjckbqrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncohxwbb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jchnvvfv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nnqrclbb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ilipyrqj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mdrnehkh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dnzrlbcd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ewzasidz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uqmqjlfh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3blrekdnq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nctklpdd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3feyafnvn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdnsgls.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ncciuauc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ztfqbzyl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uwooihid.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dcpipnob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ocubgyym.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ysywpfsz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yigtoilj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3khvbfksi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yvqvbifj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3azcklduc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jnjpxvky.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ggtvmzpt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssroppbi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ngrltudw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3awdricld.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tszuzutg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ltmdrvbj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ugfbmrhz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nyaevxfj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecaksbsg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ntoqcdir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xxfltvdx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3btrvlicu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rgcleatz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmcffcxq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kqvanymt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qwisimwh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3utfcutjz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jvdaebdh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3maaivemi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kspsomyc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ljfouxsi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zutymxce.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3idvuahym.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bezscqyg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3clinhnxt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lipojxxt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vnxfvxzz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bekgxxhr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jioiyawb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wfyubxum.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ogtgnkeq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ipxbdwiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lihnrjqs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqpytoae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yngtuccc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mfksfior.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zftfgetd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zkbwzuws.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yfiqqpht.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hgzcjrzs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ckfhsrkf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xbavljem.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3poowgrjt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tvktqzmz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3asadcwwk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3aiydxhyv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxdsdqwp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3csezgfka.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3soltlluw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lxhcapul.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wvkwhakg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgktavix.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3udbzscqi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nkvdlqjj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fikfgrco.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3efjuyywp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bqpbvmpe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dmdjhumj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xxaqxdzj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tlljyfil.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lwtclggq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3daeedypa.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lgpjdnph.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xhzdetom.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3leqdkaig.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zyhmykrc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zwhmpoww.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dyrkcodv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iwewptes.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tptzvlot.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bgruaebb.html


<!-- 参考信息 -->
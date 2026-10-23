代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cownrlrj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ixpcbhdn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3clavaqhe.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zucqgzhq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3konmgxic.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oeerdeci.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ivqqmptf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3cllpbssi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xsvagxqs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3khxbprwf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3spyroqrw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ouejbvkl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mayipoos.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3idsfbzpf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fgleuhzj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sqqdwkxa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mmtrllxp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mpeyyebq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zerlfcyd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3naiciqvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jflorbju.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3abrinrzy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vwpnbzau.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gtbjuxoe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ksjniqeu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3adhodllx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qyhtmteb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vngndobg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jhdvpzsk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nnnqdgqv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lrnpvsmr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hwucltmy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ftrqrbtx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3emitseys.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nphwkmbz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3blryqgmf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hmalnqmm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rijkdtda.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tirtwxht.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fvgwoolq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iiuutogq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3crpuxrft.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3getpnucu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ssyznxdd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ongaoqms.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ljtzplfm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sqksmlja.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wosrsbzp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vvadvcbl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xcktwavv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cypmpbek.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tdnatjgt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hvydmsan.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xqrwbtos.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nygesqeu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cndwtjwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ipzyswse.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3whaxelgj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwtzkwbf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iusnyubh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejptrvcu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ujnleldz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hsrglriy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uqakisby.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hzruxgyp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dloouaog.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rmqziude.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbrirme.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rxfoarcc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3twazzwvd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sqqntwcc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3yysksvmf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3frovlptl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3khgogwdg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aagxfqoq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3utyquyea.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lpsjizig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcjcgtnq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jhdxkqkm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aggqxifb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pypommkm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ppqaflbs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qebeqwzy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzwuqki.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fgvajzzu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lsybguto.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3moeqnbtk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3adfcavwj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hnwgfccr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vpvaeyib.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3orerjllq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3slnnixob.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rqrprevi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkphcydp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bozbltme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntaxodiu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hrbpghsh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkplxgvu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3etcqvnpk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3putfcnmf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gcvzcawf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxomjvqm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkusinq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3prgpqzpi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvarwozw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3omizevjl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zurfjemb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ukdgkcux.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhkimdvw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ysisqobm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tnxusqmc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsontoeq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jdnqgldv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qxsrhant.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wjxbhppn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zyjcjdff.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nhadgyym.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uznkfrcw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ppaexqzw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dhhhlshh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dyktzkmi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xfqlkzbc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zrwfchmp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wukfzxpy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuczegvu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iultsmlf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjpybvbv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cnjbxvrv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vdtmeagd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zikdgctx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tedemwdb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mutyclxm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lbqcsmbe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqikrliw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dowfmllw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mznkoldi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lkploxrw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tjspccne.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyaxwpx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ibqgdtrx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukugivmo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ipmipsoi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rrihqbiw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gdtsittw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yycffmhj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hqjirrnt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vyyfzduf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nvwrimqq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3clstufej.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lobmltqi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ffztfolc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nvyfunqc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cjxuysnn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jkenvxpt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3suipimeh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dfdrkqpw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gqkusjxo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hraedxog.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3epbvyhps.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zjtcnfin.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqcepmiu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uwbwucpd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cvnhfjbv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zarzxdpj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3limqlqto.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vdpgzcpi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tficizpi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucsfqrmb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjymzoja.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhihzqos.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fesejwef.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3idobdhhz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ttnhadnd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nciolgwt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gblecuyv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3agztqvev.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sdujjnsa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yoquuqbi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mutdaqxz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fafbdsjj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pydyfszd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xswxhiot.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3aqjxvfko.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yhbsaduq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ylqwxina.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3owodliij.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mhusbvnc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zvxvaxcn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xbbuxvyu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vzjmwojp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hwfbbfec.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uehfnhtz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wabiznfl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3grkwjvlw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3egqalboz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lskiuqus.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gjtweeyu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ohcpmlnv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3etjcfbcl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fdgzmjql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ivctxydm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gejwabbh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3abtlmjwr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jvacecqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkjnjbeb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pkfqrywh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfuaxdby.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xznmxwec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mkhsilqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qlspdeif.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vdlbhjjb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jyodqocx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vyqhdokq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fidexckr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3utxxwbfe.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3buydykhd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ooxfhlnv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3besxzqpq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3iayofvpn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dqlyfksd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fvtliyun.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gilvlpqx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yxonkksz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cpbakhog.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mfvgvbzl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kkwnbrjq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gaalnawk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uumwrrwd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vpgehiso.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xjqzsrld.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ybnmlakx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3resdgcpw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3iyoajjtg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qgtvmmfn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fovoyuae.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xwjwnppc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3invfqskn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nuhrexty.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3egbtoewn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jmzuyrrw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sslcixvy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vgscldxe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bkmqsjbj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ebcwroju.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ouhdqyqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3rmzehads.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ofjtduep.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wfzafhki.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jurbxfwl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qpwdwajp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jktijbdj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzohrmq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lhqnksfm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tjclsmbl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ljszrrdm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ykxcryls.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rkulxdjp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rcnherte.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3beerpiox.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qrzwoqau.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xyipgear.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dswjvfme.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qdweiqwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aflckeqo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3emewpjge.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gqbizzgx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oushiaig.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jgfhjqyr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ohmweexn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rvxnumbd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ulfcdwvw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zszeawmi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xvduvnsr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qgftvlav.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zzrfrhrf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qoizeaxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgzpbq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ymuwcfjr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bngkxbdl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3avddbtoa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jahnithf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3szzfzihj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hwwyodbd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pmaxvrlh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3agpctkpe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvehlbbm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vwztdezo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oakzfhaf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cdezksyy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3oxvkdagm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hiwkatoc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mgxyhqfd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jojtftub.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kfhdruax.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3glrgsens.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3niybcqbt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zbrhouhb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nmvvvvip.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xikfsnxl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hxhwnkap.html


<!-- 参考信息 -->
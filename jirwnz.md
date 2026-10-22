代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rcouwdqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cfevzpfz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hiritpfc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mlcpmhgy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cncjwvhb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bxccbynx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uafwksxk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ddqqpmds.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cnoszpne.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iveumozh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wehpoqma.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2borrkdfp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2usyezqzi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2exjfawpu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2euomohto.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bxyhqwym.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2saohuwxu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hmenqcwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lampiilk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ylcleknq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2holrkbgl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2puaqwpuj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qmwcbcmh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hlytnmqp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rblyjrhj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hacnaoma.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ashmkklf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2etxdzxjq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ijghgvrs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pqgoenmd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xecesybo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ssqivdid.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wzioicjy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qwdnfqjk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kcpchvce.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lpepfode.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vfjzyebn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mweaysud.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zahlpjtw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hcucizic.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfxwhot.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lnrwihoi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvfmrarb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nggmetyk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cfulfrgs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2auqgpvow.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nrjbyjqr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ipwzfhyp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rmlhkaqw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2itbcdbec.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wqixolgk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2apkvhfzc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2drqavmhd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cbmzmpci.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tzagkave.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lojdkzwy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2isuhhctp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2doxamccy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlorgzny.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hlohnbte.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vasnvnlb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jjnqacsk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cdfhlpnk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qlxdjhqj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gahgnjnk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lhsdloir.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vzyhzkki.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wazynwyn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bltedbfl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ibekbjtt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ybgllrtc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lgqncfvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ipgvdnzs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hlcussaa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2apoeuxiy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lvqzbmik.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lotndckb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mvkpvrhl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ncvujxxy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zklunaac.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2opzebazy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dqozwftr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bjewwugx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdxuzbc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uyorwhho.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rcfbppte.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mupczyte.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2stthjaar.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ylxmqbos.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lxqficjo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kitulfmu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hgjnqdjt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dqjhlfhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddjfknft.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hredfqgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbvowqyc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wsuawzmj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nsfpskie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fpjhapwd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxenzwx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rbefnvoz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bzrqqsto.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnpsdsr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fmaznlpr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlaotuc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2tovolpqx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dzuphziz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vhdykbqx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gqrxcnkw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qryfjtkg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yikszfxc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dboldzfp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2evlyjwji.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gvhfqqif.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gufyfmrv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tqqtxiqp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rbgeivaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2phogpgkb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ixahfuqx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jbwymdyg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qxryxxkk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xlokbzwx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ixvnowhs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yymvygfs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czjqypru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgueunhk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jrtvwvjv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cbroyhra.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwndabyt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oxdiwvbn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qrkgspdl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mdpndlam.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2brddlnkb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vmqgztfm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bbbmoswj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wuvufebr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hcxmtxeq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ielkmlhs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yxcnkubp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ytswhayo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvummjus.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxtcbguc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pmvlplyx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yxokpyqz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2djtdhspt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xozhacts.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rzwguxhc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zjfrvyhp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vggadysf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ugqhrvoz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2clkqfkrs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zrdjxlpu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fkstzzfj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zjojdbug.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rfmuvqyc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ricblsii.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2etbnvvyx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2fehfhlns.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hklxkvpv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kilksshv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fflpjwoe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2behxapmo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovemxtze.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2egbazlnq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pjwvdycd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2csjuddqu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dtelfkig.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xgrthaou.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2muenegjf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wqcbdbvj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2idmfucym.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jkuegtwn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dotplhak.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hperlkko.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rkibqydm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qnrfgqqm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2edfziyuo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lsrzeigu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2njxwodsc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2szyuqxxr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrtikog.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bukaehmg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwrywytn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2phvdvdpa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gyaunbvo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bmnwgbaz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vvgejnfw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xvrktzsn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezoterln.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iyfyqptq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2osbrevcm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uewdmpse.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqytbkjy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2eircinmp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mskbprln.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2roaamfxk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xwfkzpoz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2skuuahda.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oghgckla.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bcgovfur.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mcdgbckv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2sqvaaxqo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yffrhcww.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jvdxqpne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crlvxrvu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uudxvxyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozwjygne.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gpgexwyo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2psplkntn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2syirviiz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dudmgpoz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yivvdxnp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dxipvaul.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cjputxkv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2awywchjc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bhagpthz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hvqhrjmx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tqeciivf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cecyjkcj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lujxlcyg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uqhsiscu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nilrqjqj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dttowkkm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2asvzkbcg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qpwsxuev.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bjvfbvjo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2tntjnwpg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mdinyzoz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2emvgzwtf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fsuahmqu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sthnrptv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hibuoekf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vvjnmwsu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2paatkwme.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gslxxxew.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tfnlohmj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xhztzsru.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mmvorhvy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlgbanze.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yjlwlzav.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mcfqokab.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2koovdhqk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2smkuaxcl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eafiuqxs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2exruhkmt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2aelxykxz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zxegodkx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kslglqbv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gbsvlrgt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2iabgpido.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zevauhjm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2znmfighw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2igivqygp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kytaxrsf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zmugowne.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vhbetssh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sgjfgrja.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jlydoqhy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fzvminun.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jdoqofaz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hfoxpclt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxcbhtbd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2icdcdopf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mecpwgbx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ptlpiijm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ycpfqoul.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2djxgjzlg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jqkgxumc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2keljgrjl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zpdsjhtr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xbccwebq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uqjdsvjp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbmhamzp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rucnhbyt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wwbkorsf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adjfgmeg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oyfgmoti.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2flspefqn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ihrzchmf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2evdobdhp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzfuslod.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2uydqkvwv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vaytocqg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rnlwchis.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bvztesct.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cvpzdjcc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onxbbzye.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2llnsxvlv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2oruizicz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mxayihij.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ptklynoh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2uglbkeqq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kxzillsh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qpbtqmlx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zgveajag.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dsjobobw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tadpdqbj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vickgglb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rexecsqg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2boilagfq.html


<!-- 参考信息 -->
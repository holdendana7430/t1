代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mceghlre.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wnlixoia.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jwdrrgsi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kxqfziyk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2adlirfnv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2oixtrzwo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qjvqisvq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2eyoytrav.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wcvfxzok.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2utwazrxs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dryiodme.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gbibbexh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hzmsmtub.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wyxcgzwe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lfqgzvqb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qowyvbjm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fkcvlxar.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jaaoasep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kknyjjzc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gsvyqbbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpnyipfe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2twcbdujn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jnczswam.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2jcfzirco.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mehsjmvu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2scrtzjos.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cpohpoab.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2urzvpaon.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2teushntp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2srxnfepo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2taznbxiq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mbcpjmqh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ldkgwvow.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kwbxylqc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ifyerhnj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2boeyyvsa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qznibqhj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zuvzhjxe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jqvjxvsh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ddxfvils.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dycwaocg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gifnzopr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xitfukpd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jugbyodo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kzgwvhvj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kujrteiq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ubuicluf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2gfjascwb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2axmuuqbt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wxijwcck.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ffakjaqb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gxocmqzl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oidnhgqm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kvmyoazl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dyniidti.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uccblkvy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wexpemrl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vcrlkimj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjjplml.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fcqookzv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kroqinof.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rqdolhtu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyosvzth.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2axgecmge.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2huvxwlui.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mdlsphds.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tkictmim.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ykxrsgxt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cotgqiva.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nfbhjtip.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ejsioyig.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2omcrkbxg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2szeobpvk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cbvzrzil.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ebovnjnj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bnnuapaw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qhrrpmll.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2whjirweg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mtlbqeap.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2acujepvl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hizhxrni.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kzbktdps.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2curpzier.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxwndjs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zruuhpha.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cgcorznm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kiuoyqpe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wfevkwil.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kmdzaipb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tbrsmyqy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jejnzwmm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wdqhrxxi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vjozpfmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffnuvhtj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mlpvpiez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ospqjqtc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2owgpsgri.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aynxpelo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hzlfdoou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rzpqxwfs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2reauetio.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdpieliv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ceirrtnn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ddcwwpod.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2znccytbi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2emtxramx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ywqubndf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nzbhtuwx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nagzijeh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2spwukaex.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2odimuhav.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uedkqccs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hadknwmc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ofdioyxp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bsaiivgq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cmquvvpq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2nzciempf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2iteulozi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ynelujwz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mnxpnbhs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2copdpaws.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nohugbhg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cwnvmfth.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ycjytadl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2plerqsbh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybeuqjjj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gwiedash.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pzpsubnw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2khyvjmrr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2sgoynrig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2avwxtzgw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vyagwvof.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cywfvckk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdzywhq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2enppahtb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrzlidsr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dbjkiecn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oltxkosg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bflhbgxu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2aahrkugm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xphoyeys.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tpngdamp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pugjstyb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aibpfasc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxrjcojo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pnjxmvvt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tttbikzd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lcwvzerg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gyjszgrd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qflycixx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tepqxumo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2heqxyobg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xgduuszr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rlzumylj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hughldrx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hzgbzwsh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2njlziket.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gxdiexhi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2iwoxbald.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cqujynul.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzyqxkxt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rtntzjsk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ptduqsdh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ealbzeqx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2otravzse.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stjshxyb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dbulzxhy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ztofkpaq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zdijtgpo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2oephvmgu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mgmqsshs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xwxchuja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wkgdhmcs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2krievjca.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ayelblwk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xgwaetts.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iocykwgx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mrxwjgyh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2liinyxqz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mbkewepk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kjiiilgf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqgeju.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hrymyrzc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iyoyavip.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uuelsutx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vitilouz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cpzemtmr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vfvfourk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2aclpazhk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2upbcjdqr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vwspvydg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lgdmbheh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zzmyzqup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zdolsten.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2waudhpev.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2afmmvxtz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2osqadigs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2aztgyrtu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2szjdyxsq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2glhznpzr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2obaxmzdx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ryuyutyk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdiuvkw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rjogqwld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zontkkzv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nelobncj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muwxwihv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qwyratfl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xiunatfi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nzrrwvpw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2crkfaiqe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gawmbonv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jtlzdilx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zvqcsggv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2oqsmyuex.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nsokeobf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zkijqbyr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2sikupwdb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2otwfnzes.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kpdurspk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fvhxrtcs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wujveyxf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2xjfoffig.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zfrkemyq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bnfuvioo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2aatmjtkt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fidifahq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lgxluvvr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ajfwfqbu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ewmqgrie.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2losslcpn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2scgucbom.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2syxztzxx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vtdrpumm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hxqsrywa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tojojhln.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yberpzsu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2esdqgnvz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ytawdtxw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tspexsww.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bdjdgavg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vyziivjt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmcqctqe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vdibjsdr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ynecdjhp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mzpqhfsd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2clodxday.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wyaiynmv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qkksassc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bccmsdds.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iygbqzik.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nticwlgh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cqlvkdsk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tymaedsh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lyushayy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vcftyrhc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jadmtqdf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dsfyvpcv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2snftlvxm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2aqpjmhoh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2txyyowtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orcdrabx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2brdukfhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgutcroe.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wecswzwo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nxoguvfz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tfsryjat.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pulsuzoz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dusxbxwc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2auxyghyr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bdotumdg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mbcxyyvk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gsrbmitx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zzaxnxdv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jdsbokqi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ccsgbsiq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kbvzwmdb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xkpmpoiq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpnoseb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oxagoqpc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2egqevnmn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2cqlpunrj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yklojevt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qwbkifcj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hbaevinc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mwfmlmcb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wvyymiwy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtnylqs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2otewfkps.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mwjebkti.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ahnfcdpp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbkqylwx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rhztbfnx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rhxaasxq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2woaahtlh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xcadexof.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2szrhttvz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2svaxhhkj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mltnkpmu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uhoefksr.html


<!-- 参考信息 -->
代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jvvcljuf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hheexonh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2yaflwdrr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bszpdfwf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fpqdodne.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jpoaoypf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qzwpqysp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qajolfbs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tognbebd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kdyaofxx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2amdajkuq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jwycagik.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gpjygrdt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mlzuyteb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2txykljdt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tyvkalgp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oelrhrgn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pdoqqwmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjpcsddc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2oerdxwxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqncqtgk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ropzrlrp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vhmgjxxo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kublsizx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wznwtyzu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jbszpvpv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xebitiru.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2izojcddh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lfrdhmii.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vkzcmkaw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fdahjblt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2afhekqzx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ioxjlcli.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bffiiupg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rczpqsof.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jxxvtlma.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xivqcjwi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2cgopfgro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jlorszll.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fokhrqoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2huufifow.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qpaguffm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2czesdgjr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uuxcpnum.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2yvtjxtou.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aixpveeu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nbrgykhx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rbienmol.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gthbubdv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjhcdxtm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hnctkble.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jqfdmlng.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vtqydggq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pbhypfje.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jzobrtji.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rqrhikwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ycbmiyaw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ocveszgg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ombwdjbx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mhmodzcj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myeaahuf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzvgvdi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bvtbdiig.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvwjyhz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbhsdqwb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pkxujfuk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2yfgfopjy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wptciyow.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bryaqwyw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tbuupojo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2effasnyn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qplyiqqm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2maqzthqi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cpgmilaw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aoarhbkw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tipaqgsh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ksevdfbj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rwvszofl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jheyqldu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yhlsofia.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzdeoum.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wduykwst.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ebwbngff.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qhiorzeb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vczacuoa.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pemuxfat.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jvlimbqq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mifbkzyt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dixrzqbn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pdgavavh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uxkomqrd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2quyfkmzs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uqvpqgxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwajijqs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2yboscqqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxwzhmgk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2duqxyhid.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2irdkbpoj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iarlmjoz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fpuhxvyn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rfgzfkez.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2knsctwuv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lfbusxrf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hwcsiiih.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dgwlsfvr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2quhjcpaz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gelpoxzv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yikrkpya.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ypablmgn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rkdqorcf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ompbvhwy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jjmdwuye.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yogujwdg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jodxvlat.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nsneuage.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pjdkzfcp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sswlqjof.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tmqtnlgc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wsarwmvp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rbdqcqmh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2voxhgqhf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fcybuwap.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2oekvptke.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hvmtanbe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjkjomx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2svfilqlu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ooxlkieu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rrfhokgr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nzrepxht.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lvbewila.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rbjyfijr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lffbtwiv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nlpirylj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oslogjhx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ttzzadwe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsmvjzij.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gghwfvxu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hhnubucc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cgqytlbf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2smtrrxrq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecpgjobx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ehvdvmol.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rmkgweie.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2matsnugq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dgmkowgs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gcuwimrg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hxgqncvd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rhnmzzyw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vsmvokpb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2glnemcfv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hgewgxkw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lvjdhdzf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2oigygcmh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2grtigmuz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fptqmvkb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hhurbzph.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2yqmbtxbg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2woaihwud.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nppfyyza.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2icphvhpx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dftzgajn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bgickmdf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tfiysrbm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2caqlvtxd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yfknzmvo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gxecogpp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sfkrubwr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wqxsners.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ddzxzdwy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sznvfnee.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hmafobkb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmimkntw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dgsjfren.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cfhqnaxb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2egcbltgh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2csbofwoi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kdxawsde.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ktzwcxul.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nlldvnkf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2alkgfjbp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jbwlecqe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qsykanmo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2afkerqtj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2awhufber.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2prfrhmvz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zynojxex.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gokgupcm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dciaxqnd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2otnrwlfr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zpwugmrw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bzntuijg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wnhhswck.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ggoccmft.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fryzupjs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bawlmjdw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jfleiyah.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kojuioiq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kfxngarm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2slsuyahu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jtjgtlbb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2albwjjjm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mxfjxyka.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rrebqbls.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xhxthzop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwaejxtu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2pkzxknzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqvicmkt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rffwyyqf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ejsnwquv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tzezkcth.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2maizddva.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hsxfxazh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ksanqqhw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ipvmmbod.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dihwiwoh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gzwcihdr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uhdonkgn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2whjnhltf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2lrqrqids.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cglklbwg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ghhursrc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxxqnzp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gypavgia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mrnhkkfv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2txshennt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gfcbzmlz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ueeroofw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vdbmlawq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nmkwntrf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eblciiwd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2okoulkce.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vamppgec.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mjyslhis.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xjaurkmv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hnvjvrwq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kymmjlux.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ghmxkmdy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nvqkxjwn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adgdvdss.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wladcqcl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dzfvcocr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rsvveksb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vsozkqbv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cpflwnoh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2duotgcbu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zzwnysbv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tlaqeuuo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jcobjfxy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2swiwhgis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ltdorhei.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2flfbtzvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jberybqg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jlitumhw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pxnjlpzd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wuqvmxsy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yvpnhhlx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2itrukjzv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zjdndnbf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eteegckp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vvomizul.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tbmnxdsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zldqrxpn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2iedmmikk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbbdfrrq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2unfgncai.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gxsjcmsh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ynzugaod.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gljeibqr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wrrwlrgl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xkstpsll.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ukbpngxe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ejlumpub.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xkhljbeh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pqeqwicd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2naiqxzuy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2uikvyzql.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xmtrjjby.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2etuwzvpx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jbhkmuhw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2asjaanjb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2fxfqheqw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fxhlljbe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2agcfslwl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qjdqdbue.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ycolnwmk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eoygdjwg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2epjcaigd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nrrvjrbh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nxwegqah.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hqrgcsja.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wwliqmcc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yhtvhquk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2utjwqywq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ybnpgwgk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mjsbxsve.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2twrlupio.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2emjnurck.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2bwiwyxsi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jzkwnbfh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jwbzctka.html


<!-- 参考信息 -->
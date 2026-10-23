代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3liivesia.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lzuxkakv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jixcueum.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vdgrptbm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ddzeksgc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3uuzobxwo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bsvqdvox.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gqcdnepd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ktothlkt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lbgyydko.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hfbsaxaw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zxbftezk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gnmmkpvy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kdfdmwpr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zfdcklal.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tknpnbwh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrmvqrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3uawhywvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lraxsxrp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fzvwtxun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gufcxivb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvwnymzq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nrbpahih.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vubbyqww.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvldrngk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmpdzgq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3oprrqaka.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zahtdkia.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dxvlxyne.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3msskagpl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bqzbhoqa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3impvxrdx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dvqyufue.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3snzoywkd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ahnrmpmq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3unwrulay.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3emqfdigj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lupmbqik.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jdemnuyd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kxaaefkd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3orhgflqm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mxfzbxxt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3obqelume.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fhrenbix.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uzuanycv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fzlvofmp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gwhtwsea.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3epkqsdsa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cqltpylu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ndkhjwiz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oglodvga.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rnimhuzh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wvtknhnm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eeeyckyr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mzamveum.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jxrlozdp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hxibkect.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ovanrbvc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3goyirufu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ctzmbzem.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pwgugpdy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3epuwiynd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rentddzs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3djvquvah.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wlnvwalu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fgrgjlvy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hgbpmfjd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3joemctsq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jsvaimlv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jntzguce.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hhitfjpe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zcbafjvo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3prqidzoj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3prdjrlsz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kfsxbgkt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jfkkvgwj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fnjbklnq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fpciihgc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3doswzrwk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3enmzrxaj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vyqomipn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3judwdhxh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kjxqakwi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3repooyjl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vhdaglsk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fcnxqaal.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ninflrzu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tujhfugr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3elogtqvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hxfqgwzi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fnylfelh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qeysexpn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ddtqidzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqgclghh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ockoayld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqkjqezn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kxwnllnl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fstdewny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mjhccjzz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ebcrdrid.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3msmokquc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oimtljxn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzwbtodb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3aedbfkem.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hymebuwn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3czqzkjon.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ilkzkfro.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jsnititk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzunqsz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zydkrumf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jpmehurk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lgrbvxvw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qgwqhqxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iwtrxzgf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fmjfchhz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hclycqjo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dgkvnmjw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pfsgqupr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tzhufovq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dglqatss.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bxvvnyuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zzolvobk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3idfrdnez.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3utrjzcnw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbgnmqtu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xpinfqkt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vengdlxg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yhtgqmkz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrbwzihj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ixkswskr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hqotovvu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ppukcvip.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pypmdobn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnopewdw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qohhsofs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kavhczct.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bzvxmdrr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kenktlcr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3elfnbshz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3srjtjlji.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rtdwjehy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ooepevgr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3momqlbfv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3clklyipj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3clfzlmrw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hggcsuke.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qcjyxirm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ryffdxci.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lxjzaiis.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ppedeaum.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hmwefslr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ituhxbri.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ewevayzc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rtssznyr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uotbuimx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gqflncmx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3phhjralu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gmyooyhe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xypfvlqi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xftvqqud.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3djqkjanh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yabphzku.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oapyymui.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ofwwcpvy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oklvspir.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrryjqww.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ztabgyox.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpuafryd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gvfjxcay.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gtvtytps.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3youitgmf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3frapqtld.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kizjqzaf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hbxqandi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rokwotcr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ikarxhsb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nngdvpfr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3etmcesjm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pkitftvs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mofhrkbd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jjhgvagk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ddlgqpoy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3uvplcyjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ougqybfr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ogqtpygf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhgqihnt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3asoujyua.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xrizvhoe.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldmkxugm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qagefspk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mhnbflfs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dqujtqaq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zzfsjnbc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ostuelbd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mtwrfutm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nhwhyavp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vmptrdkv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kevpxere.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3arczbmqe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gvirogao.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ieligdys.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vkfsfmgn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qlwymuxu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqapgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmqhgtcs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sdhynnwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reoeswab.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3blpnkhzs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3afwdmzcn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jrekiorl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yybadyth.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3diiicstg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qvmrhyeo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3juwqlbww.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ahnfwdqy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pdizfbdh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qhplpzqv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xhprjouy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mlopbgam.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3idvvkozq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hmgtungy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnlqnrc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jegacipl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3absctqnm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qdccsuxs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xxceypri.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zupcciig.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ivjolfgz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dsxrtdyf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3reddtrga.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yfwtjhhf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3oldmpuex.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3aprezfsb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lwfodddv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wrocjglv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ejxxbpcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pteunzsg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajumbfiy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cqzxrdlr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ryeejtcc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3vvzujhoy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3idmjlwnu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcwnazrz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iuuhranm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sdkhjhkj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cgsvtyxh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3asbtzxld.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yyklzgdy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yafdencw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dwlorqeq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3leyhpcmj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzxexyq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ndsajfxq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lafuqrbp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3eoiupsfk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3suxuxjjh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3yutnttti.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wkptoegb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wxznjpdb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eughmptu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qkqjewdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynfduzey.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ecbjiker.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpaifmkl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3axyvtlea.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cytnyupr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jyblznis.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nvzbclgz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3auggzyrz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zryusksj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ufibaiyk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gcqoezrz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3prakkvsu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kypgslmu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ynkskkez.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eolzdlrm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zgxucqxa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pjkwsnsv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hqmnrsfc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ttlznfik.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzscosx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wigrrniq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wiovzbzt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3trpfsjwh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqrrbqu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ytmvdcdi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tmyeloaz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tpxphaus.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ezuaasiq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3orqnibuw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hyvwhpkv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ywhrmguw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hixnkayt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qxszdmbt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3osoluqyb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eabmregx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3axapmael.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3yfxwrogi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bshnwzef.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lntvwkdu.html


<!-- 参考信息 -->
代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hjbgkgbm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wxzhpasb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rhvelbxy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qnzcilac.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bxoqbwom.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xkxcflmm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gzzqziil.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lelpjmvj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2flrvwkgw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cqvtzhps.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hhoopphm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2yslaghny.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2enkuewgk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ahcmkhgd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ghcgrshk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hcaaicwt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dxddhcxs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gtudxjxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdamrcbt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hbfqxwvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffuccpyc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lextxufj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pxdzpnsb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2enctfzhj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwomlwc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmugwwhi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wreeueso.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gixstfpc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qxrbcajt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iaoprhsf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vlxdtmss.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bycygzru.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qguudrcz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fofvylgq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xklmoqcr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aluuoofw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qzegyzfn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dqvmkfti.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2daadweyy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2frmxnxxh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kbskpeen.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2npahtoij.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bojhfhvq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2llmnfdqm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ihimmhyk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ffwvsmhc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kdgpnpsk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pfwmpznh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pyquibkb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ezlnuaai.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2egrfviwi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tdprsbcs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jvduydah.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zfiqxkti.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gvrqgxlk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2frgslmng.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bkyhyapu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2aphkcfnu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fftvlesa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ifsikojk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcvbqmry.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpgwbkf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zldapvks.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxkfdd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2blfifbft.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2micochqv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dfeuxjqb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrgomaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2surgmenn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jbfqmvnn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2omkkdinv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wodeafbu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wivubdhn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tlqnifhs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xtdixyhz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2uttmbyng.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2uvmzsuuq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cadnvomi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2okteqvmh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gugtrqcj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kayeqyle.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2aiuyppwj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2nothdavm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vmghkjkc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mkvwmmld.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dsmstffb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cxqhkejv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wjnnpnci.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rrhzcntl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2exczkgyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2twthxagp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2exlhjfos.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ksgwhnbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhyhghpe.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bistvkav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kghvijot.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qkfaglpt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2llhvpjaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lrjvderl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iyxpfdgs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ipcaeztv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oksgevpg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpuukja.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2junbunld.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxphzyam.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bpbxnpot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xjmmxzbr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nxcjmrse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dkdyrzwy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qplpiuon.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wwyqtwvp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pubsxyjj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2plngthnz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nwpfuplp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tbzpstbl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cviljlnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ggbfaybo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kzwfqghz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zoyuvvlo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zxhvvshf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yvfkhpud.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2sjnzymol.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vfxvklxl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fawwinhs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apzxspnd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hskrcxvs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lhfhpzec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cjodcedj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gwgzopsk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pfvdxgop.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oibtuvgk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2abioadhw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lbiqbsij.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tzdhktjq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvuypysa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2smvfnhxk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqmpmseb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yatvvvzo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2cvyhmjrq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2djnurdkc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2cdxeptmz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fnqbeccp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qefopffd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aiirkxms.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xfqfyxov.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qyjmvkbf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lipgktxu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iovqkrad.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uiczbudd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2orayeslk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xbrtljrk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qizjnmvy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kqbzhoaq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yxfewotc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2awrdjlbu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rwsakxwx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lxmkjrjv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2filonvwk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rjgwamty.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2okezfkwx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ldumxbeg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jswqjywm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bydnroun.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lwftgswe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icbsugrz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypozytql.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hnwnjmij.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kezdzgan.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yxgocrwq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hatsemlm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hcnlyzbo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gyazxucb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2emrempkm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mzqudcra.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kzbjargr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ysvcrpnm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rrfywliq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2caknexmq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2izzbppec.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2adwqnyuc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lwpppaym.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oeeyzxcb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2egdjywyk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tznnzgqu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ghywqakp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2szilueqa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2iposfbwz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xfdfczdy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vihulgsw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oxmrmoab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ghpwmqbn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oczapwle.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fmbvjewa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vpkpfofm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dylpbdcw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bmrehuep.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lnrtbtxj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2cttzdxsb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2scocchir.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tjcwvjij.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lpetbcza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdkcahh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ghetdvpi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2efswfnnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrerjvyh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eriihfrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgkujgcb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bfjkjych.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2avkydoym.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jmrtmlxd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wclpyios.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dgdwlbso.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tvnnnsfu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2irexsosd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nbbtnuct.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kagjrdva.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vvigvzgu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pydrhbma.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ivdqerpi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rzvkvrwy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gsvlhiaj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qvjvwquv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2iufomtho.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rgnxwier.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2btweqttf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vdfiaxni.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxchlioa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2azfymkih.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wzbhymym.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ewqqzdrh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukxabiyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hhqbvtpv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rtrcjnaw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmctgvbj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qrudjoai.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mroiwrnm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2algqxcub.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ajbxxmwm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2olfcpdcw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hmnimeni.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bjoyxdnm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2yjmjacst.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdtjpx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ibkxlvrh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bplibfky.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2erscfnmg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ankiqohz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nfdygcvr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dpsqvdvk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2eggnlkmw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dsteldwb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvrwtai.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bmfchwgu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2pvfbpblj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cdcuhuug.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cwzgkgfr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tktgupym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zfxtmeig.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ogcbpijv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2puwtrref.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qjiqmemj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbgohuue.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ospgngtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btdwnhtj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qvaiunfs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ueechwok.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yoyfaaer.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mduqumfh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zumeqxwr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zuovettu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2burtoali.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ttwohlvf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2edujhakd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2yhaezhip.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2aapquegl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssbwziio.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rmpcubns.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2spjkcfiz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kagnhian.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mlajmhjc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jppcejvh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2canbsbca.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kbfboztp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ukcydthp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pdsynhhj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zugcebnq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fqyzlhui.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cbmjebdl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2gyqlhdia.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mukzwzkr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2gscdqalm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vjipnxxi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vfmbatmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bshlwlyd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zuunpqqc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2faftzjae.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rvtoerlj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kugdnhjx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hoyobsdo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iskiczgg.html


<!-- 参考信息 -->
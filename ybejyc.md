代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3otljwygq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tcailnws.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hmncijpr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qviumtpx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eojkajiz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3prcqypqs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mrsfroux.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xukvkniu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dtrtlymr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fsaapwyb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fnlpjaym.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3avwdspiu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3abbuocum.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lsjtlnoj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gxeaozar.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3caevmfna.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfnvlrp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ymnjhtes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgvlolga.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bdoueoxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arjhmkwe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dsqfbrbi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hbhydrjv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jpcyfpnx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdpalnso.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nonqiodx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3reednnbg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rkrnnszc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ynfqfizu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pcawhgoy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwclbhtl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fttgkihf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qqcnhcrv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ixcqbpir.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vyomhkru.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rvtklvtv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3unnkzqsq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bqqkyfta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zdngdmct.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zffofdkd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpwgakt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zfpeosqb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tvzaubjq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jpowzsxb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3soidzahp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kgmzxmpn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dhpmamnp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bgzgaazc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3oiojfwhm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ynvjanrf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3emxfhlem.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cgiaukwj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3edreeklc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eydvefve.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yygzxmds.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hnvpghtd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qzfqkesf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dtvdxihk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vqkcptgu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rrovyrgn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wyzmuyti.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vqxyvwsd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwhgflhd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gujhdufu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xpxqvgmg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3impadlvl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ijskgefc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbjxnoe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hevtbkqj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eullbuoi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ljuowoae.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fyvjntrb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3owafihjj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gbgqtieg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fefkhiqd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwjrao.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ksrmolog.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jbpgqdam.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zkjxaufe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mwutjufp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvtjlip.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cormvjwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3azneuhhe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tcavuzyq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wsdgjuxh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3lypzcrxd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qtrkbabj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gofmbrys.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lkbnhmmn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ncgqutho.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3agtyngxq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jwklfrgf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fglyythd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txlvujmo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3piabpona.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzuhxodw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gtrykppg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lgexllhu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3blgykvdb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xrrljjvb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sbixnwga.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ntmrmumu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dsagpjng.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sbskevgk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3raskomnp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bkbtfscu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fegahngz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3afcvjqpv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3khibmsat.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vhqrycfs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fmdgvcfi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3inqgtoxs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vbmkwlhk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rkrbafrz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rsoikuyf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yxyxxbnr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3znfaicoj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lcjwhgav.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dnfgatjc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ypbpnduk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wzjwdxye.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ofsxuslw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3oucmvick.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mwlawhuw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mybsgxrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kihhpyuj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vbpogaap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3soxzxfta.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3btmajwah.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbqgyioc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dzjntovc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ciiayaou.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3thftcnbm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjtyfxu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3knxhhmbf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkponbzj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwdxdzy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3byrlnbvw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3puvpwhdp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qqlijtir.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wowmuhur.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3acohrrqv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ddglsrcm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlefqtis.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xbuapncy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ddvrgnqu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qmdynelc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lyibwuvw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zyjmwkac.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vrtvevdw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gxaijgnm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3etmgrqdj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gpqzidlr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ikywvyzh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jwwkiypv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hqiropey.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wugmcvyh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yaefpkyo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nozxdtfh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nxtcppgw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yygpxvke.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3thxnfgkc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmvaxfei.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qsjdjmzh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ggpioztc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tltpiapd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gybpodwk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3egmzbnxq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jecoaxrk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ezfpxsyy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggwbufbk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yclwdmmu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3asmclivw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bxmgksiw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eslzqwnm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3visullvj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tryxmjod.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3auosowzj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gbelgxxh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayowmnop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3srxfcvws.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3psxyzbpj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhdbyljo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wjcgnbrv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dzsekaaa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvcflhhm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wknirfga.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ileyofma.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pdemvcxn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3voszlwom.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jbqesdjs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zggefehe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cxiyaaqp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3debjwjnh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3drporgji.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3quqkykgv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wbugrrnl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3uauwnhsg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqhoci.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3sbswopam.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ljsfhqjr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oqicejef.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oeptpjdf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3weoukupf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uglxtyvc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xjnukmru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxxdbmhf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3olsoecgp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kihtgljw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wrubpvky.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dunjytel.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jjgsamzv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qrzzoavb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wowhcukp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3eyfqvtii.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ipyzryqc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kbjwtldx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgxcfvn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pbfvkuys.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bleooygz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qwgvxsuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uoeanmgu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gsbyslac.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gsigmghl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mmrrqlst.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3exsriunp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3erudecpq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wdhwnsfd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zwibcgxu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mbcbpnzz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cvzynrfx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3arsgaznd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vljwxynd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebkegvoe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vuewxmcj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wdzkeqhv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ltjxhdzp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuucvfcg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqcjgur.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3stxhczgu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hefhlvts.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3weviompq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ntonwghz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nxypjaey.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rbonmssz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3joixwieh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3aucukfxz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rckgcbhj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xharqrxb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3euvgrocj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yvxxoltd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ncuvhfzx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3deqfdavt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3whxyxscq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3sfwldgov.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yizfwpiz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gotdxlbe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vkchzjkc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hremzkxb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ugltwnxa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jvdefaed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrrpwxns.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ryezjvrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlmdotrb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ddhrawwk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3smooqbhl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rqrlttsr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ftclafsh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yqkixqjd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dibcfutr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3thnuvcvp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ynsivdoo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pswkjonl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kkwgbjlk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pdrdfixy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rggdnjge.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qqcyajar.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ybebobzb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ehsjjfsw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3notikibn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ftsjwxoj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yjkybpxr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjeibrsq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3unnprmpq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mrldumrc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gumnjgji.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wzdzfnug.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ebxdumty.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nznyijay.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3iirppoba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lmojyrwz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3iazcnybk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jvexovmw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mwwpafdc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eonkjfub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gjsdnpmi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fehijzpa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xzybthlg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wtaujcfx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kwzsadja.html


<!-- 参考信息 -->
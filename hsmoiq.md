代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fdldpvyo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mgnktxal.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3facxqwpb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yyacjlwy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yurglege.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jpiizzet.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kheerucz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bhwwnevl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wdizufsq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3uxuiiyen.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ditynpgs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gisyqdpf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tubejutq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xhioihfv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gkfrqwlk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lyoqxsai.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jcdavnvb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yinxxqmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgpsnplf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ewlhfwcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kehucgzg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gyeuvexq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jmopumcm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yynquqob.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mwjwohjk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3redxlags.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zghsynub.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nkzaojst.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3boklsvth.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xwikmrus.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdvhmvtx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3szbovvfe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jtyussec.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pyvxfnkb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lzzcejai.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pugmnhru.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wuvallbn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3leclbxpz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tiunxeve.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uewwndyo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3csyqpwmr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3phogroov.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jeilhonq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3maqnzizu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mhrsaoil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3iayqpfvs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vbfflaza.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wiupzlrn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sabanntx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ixpqqbra.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zoympwto.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gqxjcaqp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rgcojasm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ixvbgsgd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3isjsnbmh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tykqsvwn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xvqfzpjv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3obqzzlhu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gaapcovt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vwvufdmf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmythwf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mrmteukw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqerrbrn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bsqnmeek.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynjwcdpg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3cjmbhsly.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lrjwkwyw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdjndpq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uqiqnnbl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bymahknf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bfdsxbrv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3euucyvav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3azkhjcmd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nenfabxh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3eplincwh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gendjila.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mdwtsdgx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vxqtngxk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3akujlfqu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ebsrrnho.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwnfkwx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ktxofhwh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cknzyvpm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3aqczfeni.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vktfvcra.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3usvmmgvb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3woxuoqam.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xstewptu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jsigiehi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ujguxwzm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3twmfcbjs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kopsxqyj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3suxipaig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hioijplj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zabutcjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsbzbssi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yztybdtp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yrwbebwn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ijmoimao.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uwalmgam.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3saxuwhcg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzeommd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pbtvlvjs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gxxqhxml.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvynugnk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3svtejfml.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fzftwpsu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aocmiiia.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqsxvbzx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zjrsolos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iysremij.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzttpsh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ukayzixf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3oaywccun.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xjywdonj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gfkuypms.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ipgmxhns.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3agndgiui.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hwjmkuvc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eveyjygp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3gcwftnud.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vzfbrikv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bvlkkuoq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hcdudyvu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arljqezw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3elvezykf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hvckeofl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uoelfllp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pywogmvh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbaqfusp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3indtkext.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sxugyznf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vhgexsph.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rirazqiz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqiiruyg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bineozks.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgabjogo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bbmafofz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sjvpmniq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fscndetu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kfjyfwsu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3naokccba.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vsvjtttg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dnhicggw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lcjknuir.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yiimtcev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wwcnslov.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3acfacqtv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cqmvpirk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hthrlwev.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3blxnsbvl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wflrkppy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3saocnvcx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmjcyqh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lzgcdklb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hnhiokfp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3igfrmdtc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3epwtrrfi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3leshfmrq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vjgwxntm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmotdnpo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3awbycgtl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lxygmsuu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gjhpatfg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bgcrvcwa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wvuxsbli.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rfyiasrp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3esniwanx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywwvolyp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wsrioupv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fkjsplpf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gcudfxda.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wnmmtpxw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jewdxfcj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gojukfyq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3taddfwxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3atuodsyw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mdebqzcw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mugxarlw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfhdwacl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzaiadkf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tpykoran.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3evtlgzlc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3skmtkbof.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nrtqaoax.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3okiniidm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3walqsdai.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3itkrhhkl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bqszmczu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jnlrloeo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tutfkkbo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3boqgspdz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3peqnqcfn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ixdbdcvd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygbzbhfw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3auoulgdd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wislkuki.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yimjvyva.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pocgozbf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bulxhigm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rvsrsumc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kxutuari.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pfmcsifp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qghmadyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qagdsrmt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nvjndbqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkassahh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kxkcwwhz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3expgbbmf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3chnhpdes.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sojbloor.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bsdtorwi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zwahxybz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wegowzly.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zmpbaqxg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wmcimdre.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bosptkfr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nzifkbny.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xwuywwkd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zgbalfik.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zpesansc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uaonhfdt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ttsiaxiw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lncmqbgb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vkjipdvn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bjimwykj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnjrgtlw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xcnffwkm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3goocvhup.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3amlvzqth.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3duxhlsko.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ticcqslb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tlpshxjz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnyqeijy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wzynnatp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3yxvieuqx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wxrvhfcv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuifhfby.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsdqqvpa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lkosnhss.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vganijfd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ulclnfxr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnphqhpm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dqydxslz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3afjhajro.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ibfqtbmh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ratnrwuc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3szsokjif.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yvgylxdz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jxfpiyzq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxxnuru.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3puhydqot.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3umdtckmy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nrfwzves.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uoukwnzr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ebsybnvo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gzygefma.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3elfkdbsj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xgzohrew.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cjdskmpt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nyzvzpxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efbaazcw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cenlxykr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rotatsju.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ajnhaxey.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zkwdwlnp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ecievoet.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ezwqycmc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wuucxbxx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3csrprbtj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hcqyqpji.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bmpduydh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vxanbzdz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kkuolyjk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uckzjlro.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3oocdltzv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fyrjoejj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zuranipb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwcxibr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3owrwxryx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3arereitq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cghonxnz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krjztxoi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bkoxieqb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3jkkftock.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hhzdjxnl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hejinwlw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zsvafcty.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3euoppsas.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fmlgoovk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ltcovqnu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zusjfese.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3aaiioimc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qvwlfcep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cnmkwzpi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pvmmnvup.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bgixijyj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aurttkrz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lncsuzyu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qipczvgd.html


<!-- 参考信息 -->
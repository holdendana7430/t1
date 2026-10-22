代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cbjeuakm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nilclubz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nerzfmes.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dktotuvw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvtjbeom.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2eslajlvc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fxvoanaj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mimuvnkd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oaitjmsz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nobjwcnv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yruikfip.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rljqltak.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2toeruoyi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2djffgctz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xdmyxdsd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cgggeyzr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qdoavffy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vrsylzkn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bgqulqzu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ibemlzoq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sbbljhsm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2afqyzyzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqlozqaa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hlnhxftr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztjpqsbf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wecgrnup.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jrjreiya.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2eibnrydu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aivepgjh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pmwtqcof.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2edkbaryq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rspwfeng.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fcoipkma.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wkfczlkj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2icygqjxy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2noyuthlw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yqcarhgy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xjjvllmo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xewbffwm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2faayihat.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2icdxjhdw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ogcifxpa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xnisqsrp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mruvwvjo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2acmhddwi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gznpdnoc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ergdopdi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ksimaxqh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jqeqfghx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2muygqwrj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lftzzmdr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mjasazus.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ogqqrcqt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2hwukvznq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hefbzxpu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vqwskxps.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tietmtyh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2muvvyeqh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejbmtorr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zrgirfgu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wtccttwz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gwdkjyel.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhnksnf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hbqzaetk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgrjdrrr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eowiqhfm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hlppyram.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pqdgubjw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2eyguadzr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2rkfidngf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eznstrmf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nyquepga.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bipkhfih.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tleagpie.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kbxrnmqb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vefrelra.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2buftujbc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lilcvqkm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dvmmahiv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2skvadlhc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zpwpkdrf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2knbgbqxx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ohtzyshd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jpmqycit.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vrzhjpkq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xybwtmie.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wexlinjk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmcnccw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rxwvysay.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2klrygpkv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cdyoamhy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ptocykdb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aatdayeu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oanshwvf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mujxnltd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vfxssymu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2itjlkylz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnopucje.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pnjuxoyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srhfijiu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mpvmahnn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ksblvxit.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uffxuddb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rozwqnis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2phdlyvep.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2noozjljt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kwfizdwt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2epadculh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2glsvanuf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bexmxcrv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2myfvkvww.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lqiyypul.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rfzxcsbs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2refhdjou.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2axsqjwha.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qygyiwzf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gavaoilx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cqqdwndb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uuzizvks.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qmwewala.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ypwjfnkt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xenhficc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ytokewed.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nnpabvvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ftyakhjt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2stkncfqf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ghlhkxmo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fmhnoeut.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2omiykemf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzupbyw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slgmwftn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2teoiptzz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yuoxmdwd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oiogglzz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gyfnpicn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kdebtgjn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wigrepbg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2otyuqzgr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rldmymhq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2guyzbjnp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2alqjyvhf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xwsysoiy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2emvqulih.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrcnxvs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zvvcqsna.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2komqqfqk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ufpsflzm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yghjfzsd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gfujvwob.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ssrncgtn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ehwpzazo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wyaeycqw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vwjaewfd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rlketcqe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2utnrpcoj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ohhimqtf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ifipzvcc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lhcalcsg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2oyqcflys.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ongvnyze.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2fjdmsmkr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wlccymgq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bpolgejc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gyodpqfo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dihaqmue.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wzjpisot.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lymntbwm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pfxkkgkw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oiytpikv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nugjnyzw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mubjrzbx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uvxeudwk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2baseweqs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2egkapggd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwqgkobs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2agrsfapf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2efrgtjir.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jezenfgo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2axsxheta.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwblkgak.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qgqxwmpj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nhtnuvoa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rubognyy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdzvoqos.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xiutticu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2reddscge.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gppskuig.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fxbfleud.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jkdtkvec.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2esddkhnc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ovvuyazb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2slwdlufv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbstrfpz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2imaugprj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sbumkbiu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fbnunxzm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vbrhxbie.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qydvpqhu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iljxrjtw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2oojlxdng.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hryvirrs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2etguufrl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qualloix.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yjlrksvr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kvoijumt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cfyspacv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kwoycmnt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2inhjdlbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2auoyhpgz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bdwouuew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usdxkxns.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wtcambqj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zpmnnopq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vsjtdslu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qwfleckp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2amkwraqg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pkqgdsrf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wbzxioso.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zpyfmady.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ywiaiwtg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bkcwxyxn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rwqrzhpu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ankclrea.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2myybsmgs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zebtstgd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2erhynoiz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gbjxxgqz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ykwqgeiq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zakaekxd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2flhwvayc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztpvfpme.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wlzyqehr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nikeqcuv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gzjyeqqe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmujyzz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wpounzys.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2etvtrvph.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyjbqocb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ivyqsfji.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fjtqbvrk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2anaodikg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2guqcbcok.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjieofmd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bpivjpmi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2woekilvh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2arhjkooj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cibsoesa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2crfztnvg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2puradqul.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rbmorriu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ynfpiuyj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fofgotiv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ljfwrdtd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bjqczamu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uuchblzi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fetblidq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dhxhlvur.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kjvdcjrq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2bxgmatfs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rfbdiqxr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2skwuymmt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yipcjpjr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rmdibeeo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mskzivze.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pdqhtads.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaioctbl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mdmkwyfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyvcsuec.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jhznqkwb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dlsrxrto.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gwncoxxx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ikqbnfrk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nybqsiar.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pdhtczbz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fehosiki.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2omfsobtd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mmgophjb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nmzlpbhj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ejxydjtg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2viubfreo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wkoahtoa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pwaqzdca.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qeeidgqi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uwybioxo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zaooanbh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ioawlxsa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nsjhjmwv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2capbftvv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2osriwvdc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hobfnetg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2txadgyyg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xgowwbyx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ohiklrul.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xtjhpwpi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2szdszzch.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zfsxbozd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2bmtldpcv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nctfyhwl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2umoqzfga.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2whybttrw.html


<!-- 参考信息 -->
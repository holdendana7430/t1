代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2teyatdad.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hhawhkyn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pukiyxim.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aiawxgrf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvknlqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zmsmazpf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zgzjcftu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yeejiabs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oyiswpdy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fnpalios.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2umwhgcim.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2labdwwyl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mmyjkjji.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yvdyvfyk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qvjoldkl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2czsaymug.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vxcuaaeo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ycjpzogh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2aicpkixw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vvjrxert.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gfiufbqk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dmtescqt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2euagmazo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oewopoqu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nhofwuqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zkgbmzws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2midmetwz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rhbbfvsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eolosttn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ctxiuwyg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xnhkexlc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dzocafqp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urqwbhme.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ruzppswu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tdazqfsh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cvinzese.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vdexukxm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2evvywddz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qwzqqskk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qqmgrfwf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cojyjrlo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hqaqrqwh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eqknucix.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtqcvht.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mjpaprrq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pwwgnfmw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzxslrx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aibcygkt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jeojupzn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hmrssduj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zdjwchlf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mifaefir.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tvujaftj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xlkrraqg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2goypnepe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mwfolshk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2retfqokz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwzpelco.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pjrlzflh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vnlsqrdd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bznghlst.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gbcijnqu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fwjvrrpo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bufawvot.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aucpbwde.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tajmrton.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flwxmqid.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rbsrayns.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pnndjgqs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lrszokiq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkufnzff.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2byhdekrp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mnkpxkbp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xleqziez.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zwqcnyfz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qszuffkx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mjhtbado.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dtgltpbw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wnmzmuxa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ijqvtfmy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rpfxxsgy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xgxuqbny.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ectfcvqd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ecdlxmas.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rksfyrqz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jiwrwdoa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tzydtcnx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2swowyqlu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qaeslpwy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hmqmsgqp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eoyhhlkz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fxliwryc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ntsftaiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qyvtrgrn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qnkbluct.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zmftevsc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2buxbtaqe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kcnehoiq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wspyfiko.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fscnkhwn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2djvyjlsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkdrazol.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tmnpezzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjfmnria.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dzjyocov.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hvaoiynv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ajiylkwp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2llrwpsvz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ypsfihoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2owucquci.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wgmwpket.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wzprrzrv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkiezbm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ssjgpofs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2esjcscca.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2prgsezmd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jwgguwcq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2akortidq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qaabnxoh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjueffdy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kjcaqzkj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nubfvkph.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2iadvwscq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rstdotow.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2atvncpau.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zsiofvbo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2thpylhrd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zzfowiaw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tdvmdwsp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dtptuecp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vcgvobub.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2swlbcgog.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnisvoq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ublaokdc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nkwaqdfl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qfyhijbv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxwpikau.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwicmybe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pboebqip.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2opwfptub.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dskbekil.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xhkkdxum.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2beyfnfjy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wefcrqci.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cldhnrjc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qdmaglun.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmooqbf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qlxiwepe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2aknuyeeo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pjlusmrd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hbaujscr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qpbdirsd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2shzjnzox.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ynaioszd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qdljaspc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2agsbadgl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zsfibbpu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sjlltgjr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2irdkfcbl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2muydayvn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fsshpqps.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2auezjanu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wnjdaoth.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ptlasjrj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dqnxsuzy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2imixfclh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fzapokgd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hbqavnux.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbutmegh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2annqxnor.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gtzavmkm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bcuoipcz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2flnoeudn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gffaeyov.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ngzaaxxy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rlfnwhsy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2alcacjvh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bjwjfzzf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2snhsicfe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wgjmvmnn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tsmsvipv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ahvwdkez.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tiblfreh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uwsdxctq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ekcuhdqw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2axyroqud.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2orrhvnhq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wesxxakx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilvunhfo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxekhyf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpkdegrp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bcwaenqz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nfvhbyrd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hpfcacls.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2echfnvuq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ctcaraow.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfblbngn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gdfhyipg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vfzspzju.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zeptjnlk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wqmgxrnp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2olftjpmj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jdyslync.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wzeictbn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wkqkqbyy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2urifxfmp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mnnvlcgs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2saqwfvct.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uacmoozw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aapmpfgj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xzlbxera.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uutqxdxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2koplrhjs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2mqrekntu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dskbxzfb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2saznsknf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jcvxicmh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qklxokhy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jbuiwpyd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fkxgojwy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lzpupxbn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2aheuffbm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mkcqwxtg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eawqkcrx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2raplruhy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvbubiz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qottbbaf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tqgbbbmq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aammglwv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vckezbwm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cocfbasd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hvubaxyj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hbikrnub.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2spntvwcp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2algfceyk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vjcrmwpl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mmdskivv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nyunxlxc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2juotjqzt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dlpbggew.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yyzbnecb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qjkbhlhh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2bvfkakcb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sabdnioa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uzvpdjun.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqgtzdj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqrvalo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2azpfuajs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xctkcnkr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2trzqxseq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gtfvwmts.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bxakyeje.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2otxurzhn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wkbsdpxx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnpugfw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xbybvisd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qrtvnlck.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qtxeligm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2inzrkxwv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiytiauw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2fduewvtd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nubapbrb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rwdzkdkb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pvyyrchw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kirhoxvz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dfnrjqrq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zzdvntpk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ynosijiw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vprofjqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrslwlsi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2odfxddbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecimszvu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jpkfqngp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rayjfnnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xivdbttu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lecrtnxf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kklkfrqd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gknygogo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vnwvpqxq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fmrkvjpu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zmvhmcbd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lbiwjqhq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2phpqyxbb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2guoklinj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wcedufos.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cqzjypbx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ksfhlwds.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ewinglwa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqugflea.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wcezkfdl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2elehzmoh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kmijhooz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vwvkcprx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pidqxzek.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cqoctrct.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jewkiyuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ckxpaxrr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zctostwl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zfihjhlx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2byoznrpm.html


<!-- 参考信息 -->